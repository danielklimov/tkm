Migration Plan
===============

Approach
---------

### Introduction ###

The general approach to migration is to implement it in the same way
as Data Warehouses are built. The main principles are:

1. Create a temporary so called 'Data Warehouse' (DWH) to serve as a hub
   where all data is loaded, all the cleansing transformations take place.
   'DWH' may be just a few separate schemas in the target database.
   After successful migration DWH is discarded.
1. Use Change Data Capture (CDC) techniques to pull deltas (increments) from data sources
   where possible. Small tables are fully reloaded every time, changed records are marked by
   comparing new and old versions of records.
2. Data goes through several staging 'layers' until it reaches the final migrated state.
3. One Data Integration (DI) process updates only one target table.
4. Standardized logic is used to migrate data from sources to 'DWH'. Most of the DI code
   is generated automatically from table metadata.
5. Extract, load, transform (ELT) aproach is used to do the transformation.
   It means that all data transformations are done as the last step, all transformation code is written in SQL.

### Requirements: sources and targets ###

There are 2 kinds of data that must be migrated:

1. Database tables in 2 PostgreSQL databases - QVP and SVP.
2. Files in OCI object storage for QVP and SVP. File are used as attachments to other database entities,
   e.g. verification request reports, certificates, invoices etc.

Targets:

1. Unified PostgreSQL database - UniPACC.
2. Unified OCI object storage for file attachments from QVP and SVP.

Note: All the files are going to be actually copied to the new OCI object storage bucket
during migration. New UniPACC tables will not be referencing files in old OCI buckets.

### Loading Source Data ###

Data are going to be moved from source systems to the new 'DWH' in two phases:

1. Bulk migration - all data from all tables, all files are moved to the target storage.
2. Incremental migration(s) - periodical extraction of new/changed data
   from source tables and from OCI object storage.

This approach provides some room for error during every step
of migration. It reduces load on source databases. It allows
to separate the transformation part from the data loading part and allows
to run transformations over and over again until they produce clean results.

### Cutover Plan ###

After successful bulk migration and several incremental migrations, 
a set of test queries is run on source and target databases to ensure that
all data have been copied, certain key indicators match each other on source and target databases.
Uni PACC application is tested with several test user accounts to make sure
there is no errors in column values, foreign keys, the semantics of the data model is not
damaged, UI works as expected, all attached files are accessible.

When there is no more errors, source applications go offline,
the last incremental load is run and the target UniPACC goes online.

### Data Layers ###

The steps to move data from source DBs to the target DB:

1. Extract changed records, save them to OCI object storage (OCI Layer) as a csv file (gzipped).
2. Read a csv file from OCI Layer, load it into a temporary table in the 'Staging Area' (STG)
   of the 'DWH'.
3. Read a temporary table in the STG area, merge it into the permanent table in the
   same STG area with updated/inserted/deleted timestamps. Track if records were actually changed.
   A permanent table in STG area becomes a copy of the source table with the addition of timestamp
   columns that mark if there really were any changes.
4. Select data from permanent tables in the STG area, transform them
   as needed with SQL. Merge results of the transformation into the final table in the
   final schema - Business Layer (BL).

After each step data ends up in one of three layers:

1. OCI Staging layer (OCI) - source data as gzipped csv files.
2. DWH staging layer (STG)  - copies of data from source systems with added timestamps.
3. Business layer (BL) - data transformed to Uni PACC data model format.

### Data Integration Processes ###

A Data Integration (DI) process is a self-contained unit of work. It may consist
of one or more steps that are scheduled to run as one job.

There are two kinds of DI processes:

1. Source to STG. Reads 1 source table, saves file to OCI. Reads it, loads to STG,
   updates one permanent table in STG layer.
2. STG to BL. Updates one table in BL layer using one or more tables in STG as data source.
   It does either an incremental update or full reload of the target table.

Note: It is possible to query source DB and write data directly to STG
without intermediary file storage in OCI, but it is not a reliable option.
A connection to one of the two databasese may fail,
the target connections may be slow and hold back the source connection.
It's better to have a copy of all source data as files, which allows to 'replay'
the whole migration if needed without quering data in the source databases.

DI Processes can be launched independently of each other and they do not
depend on other DI processes - they are *stateless*.

Any DI process can be launched multiple times without any negative consequences.
It either updates the target table with fresh data, or does nothing if there is no
changes in source data.

Processes can be grouped and launched simultaneously in parallel as a group.

Processes or groups of processes can be launched sequentially to form a 'pipeline'.
Pipelines can be useful for correcting errors and doing other administrative tasks.
They can also be used to maintain dependencies between target tables,
e.g. update several STG tables, then update BL tables that depend on them.

The whole system of DI processes is designed in such a way that if any process fails,
it does not cause other processess to fail.
The only negative result of an error is that the target table of the DI process
will not include updated data. After the error has been corrected,
all dependent target tables come to the correct state after the next update.

Recommended Tools
------------------

The approach described above can be implemented using different tools with
variable degree of success.

One tool that fits the above requirements perfectly is Apache Airflow.
For the sake of clarity all further description is based on the assumption
that the migration is implemented using Apache Airflow as the core DI machine.

The choice of Airflow is based on the following factors:

1. Airflow is a mature DI platform well-supported in the industry.
   Due to this fact there is a lot of information, experience,
   components, approaches and best practices.
2. DI process in Airflow is called a 'Directed Acyclic Graph' (DAG).
   A DAG is a simple python file that contains definitions of so-called
   'Operators' (steps) to be called and the definition of a sequence of steps (the pipeline).
   As such, Airflow is a code-based, rather than UI-based tool, which makes it
   git-friendly, code-generation-friendly and does not require a special GUI editor - any text editor will do.
4. Airflow naturally integrates into Git, git flow and CI/CD processes.
   Airflow scheduler automatically reloads DAG definitions when they change which makes CI/CD 
   deployment trivial.
5. The required Airflow 'Operators', i.e. OCI/S3 readers/writers, PostgreSQL loaders etc.
   are readily available as open source Airflow libraries (called 'providers').
   No custom coding for this is necessary.
6. Custom specialized Airflow operators are easy to implement if needed.
7. Airflow scales from a single-node cluster to multiple-node cluster. Different
   tasks (steps) of th same DAG can be executed on different worker nodes of the cluster.
8. It has web interface for launching/stopping/monitoring processes.
9. It has a built-in secret storage for storing connection credentials that
   allows users to launch and monitor processes but not be able
   to see connection passwords.
10. It has command-line and web API interfaces and can be controlled programmatically.
11. It can be installed on a developer's laptop as 'Airflow standalone'.
    It can make development process much more flexible.

After initial configuration of Airflow and setting up DAG generation to handle STG processes,
all custom coding that is required is BL transformations
and all transformations are written as SQL statements
executed by an 'ExecuteSQL' operator.

Data Integration Diagram
------------------------------

![Migration Architecture Diagram](img/data-migr-arch.png)


Environments
-------------

There are two environments set up for the project:

1. DEV - development and testing.
2. PROD - production.

Each environment includes:

1. OCI bucket(s) for storage of file attachments and temporary files.
2. Target PostgreSQL database.
3. A virtual machine for Airflow components.

One git repository is required for the project, it works for
both DEV and PROD environments.

Development process
-------------------------

'Airflow Standalone' can be installed on developers' own workstations
either directy or as a Docker image.
In this case the development and testing is done without deploying
anything to DEV Airflow server. The developer workstation must either have 
a direct access to the target UniPACC database in DEV environment,
or the developer must install a local PostrgreSQL instance.

The common DEV Airflow cluster is used for testing.
The developer must push his changes to the dev branch in git repository,
after which the CI/CD process is triggered and the changes deployed
to dev Airflow cluster.

Preparing Test Data
---------------------

In order to write SQL transformations efficiently, developers need test data.
Test data should closely resemble production data in terms of size, distribution
of values in a coulmn, errors, null values and other discrepancies. The best option
is to use real production data that has been obfuscated - sensitive and confidential
data has been hashed or replaced wth random values.
A set of csv files for testing is prepared in DEV OCI layer in the same way as it is done during
PROD STG processes, except that data in the fields containing sensitive information
is obfuscated.

A set of obfuscation STG DAGs is genenerated in the same way as PROD DAGs.
Each DAG selects source data with obfuscation of several types is applied
to certain fields. E.g.:

FIELD NAME       | OBFUSCATION TYPE    | RESULT
-----------------|---------------------|-------------
phone_number     | phone               | `985***12`
first_name       | hash                | `a0145d67c`
email            | email               | `a21@g***.com`

Obfuscated files are also loaded into STG layer in DEV environment.

Change Data Capture (CDC)
--------------------------

### CDC for tables ###

Most of the big tables in QVP and SVP have timestamp columns `created_at`, `updated_at`
and `deleted_at`. These columns can be used to track new and changed records.
Small tables can be fully reloaded at each run. For big tables
changes for the last several days (e.g. last 7 days) are captured at each run.
Jobs are scheduled to run once a day. This approach delivers changed records with 
overlap of 6 days of changes, meaning that each change is loaded 7 times.
Records in target STG tables are updated only if record data has actually changed.

### CDC for files ###

Files that are attached to documents are described in QVP and SVP in these tables:

- QVP - `file_storage`;
- SVP - `active_storage_blobs`.

Both tables have timestamp column `created_at` that can be used to track new files.

The DAG that loads files to OCI layer can be built like this:

1. Select paths to all files that have `created_at >= current_timestamp + interval '-2 day'`.
2. Copy all these files to OCI layer.

If the DAG is scheduled to run once a day, at each run it can select all files that were
created during last 2 days. Thus, every file is loaded twice or at least once.
If the DAG failed and the error wasn't noticed for 24 hours, the file will still be loaded
at the next run.

### Automatic CDC Intervals ###

It is possible to get last changed timestamp from the target table
and then select only those records that have `updated_at > target_last_change_date`.

Pros: 

- no need to load one record several times, it saves CPU and network resources;
- if the scheduler wasn't running the job for several days, the gap will be covered in one run
  automatically.

Cons:

- More complicated logic is built into the DAG.
- The load on source system is less predictable because the size of the dataset
  to be unloaded may change.

