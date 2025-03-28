Migration Plan
===============

Approach
---------

The general approach to migration is to implement it in the same way
as Data Warehouses are implemented, based on these principles:

1. Using changed data capture (CDC) and incremental updates to pull data from data sources.
2. Data is split into several 'layers' along the migration path.
3. One data integration (DI) process updates one target table.
4. Uniform migration logic for all tables that allows to generate most of the DI code
   automatically from table definition.
5. Extract, load, transform (ELT) principle, meaning that data transformations
   are done as the last step, and all transformation logic is defined in SQL.

### Requirements and assumptions ###

There are 2 kinds of data that must be migrated:

1. Database tables in 2 PostgreSQL databases - QVP and SVP.
2. Files in OCI object storage for QVP and SVP that act as attachments to other database entities,
   e.g. verification request reports, certificates, invoices etc.

Target storage:

1. 1 PostgreSQL database - UniPACC.
2. OCI object storage for file attachments.

All the attachment files are going to be actually copied to the new OCI object storage bucket
during migration.

### Incremental Loads ###

Data are going to be moved in two phases:

1. Bulk migration - all data from all tables, all files are moved to the target storages.
2. Incremental migration - periodical extraction of new/changed data
   from source tables and from OCI object storage.

This approach allows for smooth operation,
provides room for error during every step of migration and
reduces load on source databases.

### Cutover Plan ###

After successful bulk migration and several incremental migrations, 
a set of test queries are run on source and target databases to ensure that
all data have been copied, certain key indicators match each other on source and target databases.
Uni PACC application is tested with several test user accounts
to make sure there is no errors in relationships between tables, semantics of the data model is not
damaged during migration, all attached files are accessible.

When there is no more errors, source applications go offline,
the last incremental load is executed and the target system goes online.

### Data Layers ###

These are the steps to move data from source DBs to the target DB:

1. Extract changed records, move them to OCI object storage in gzipped csv files.
2. Read a file from OCI object storage, load it into a temporary table in the 'staging area'
   of the target database.
3. Read temporary table in the 'staging area', merge it into the permanent table in the
   same 'staging area' with updated/inserted/deleted timestamps.
3. Select data from tables in the staging area in the target database, transform them
   as needed and merge results of the transformation into the final table.

After each step data ends up in one of three 'data layers':

1. OCI Staging layer (OCI) - source data in gzipped csv files.
2. Target DB staging layer (STG)  - copies of data from source systems with added timestamps.
3. Business layer (BL) - data transformed to Uni PACC data model.

### DI Processes ###

There are two kinds of DI processes:

1. STG - updates one table in STG layer.
2. BL - updates one table in BL layer.

Processes can be launched independently of each other.

Any process can be launched multiple times without any negative consequences.
It either updates the target table if fresh source data is available, or
not if there is no fresh data.

Processes can be grouped and launched in parallel as a group.

Processes or groups of processes can be chained and launched one after another
to form a 'pipeline'. Each link of the pipeline still can be launched
independently without causing any problem.

Tools
------

The approach described above can be implemented using different tools.
However, for the sake of clarity all further description is based on the assumption
that it is implemented using Apache Airflow as the core integration machine.

The choice of Airflow is based by the following factors:

1. Airflow is a mature professional level DI system well-proven in the industry;
2. Airflow DI process or 'DAG' is defined in a simple python file. Usually
   it is a trivial python file with only definitions but without any actual algorithms in it.
3. With Airflow there are many ways to generate hundreds of uniform DAGs using simple
   JSON or YAML config files. Therefore it significantly reduces the time spent
   actually coding.
4. Airflow integrates smoothly into Git, git flow and CI/CD processes.
5. All the required Airflow libraries, that contain
   DB connectors, OCI/S3 readers/writers etc. are available as open source 
   python modules.
6. Custom extensions to Airflow are easy to implement as python modules.
7. Airflow scales well from a single-node cluster to multiple-node cluster.
8. It has a web interface for launching/stopping/monitoring processes.
9. It has a built-in secret storage for storing connection credentials that
   allows tech support users to launch and monitor processes but not be able
   to see connection passwords.
9. It has command-line and web API interfaces.

Data Integration Architecture
------------------------------

### Diagram ###

![Migration Architecture Diagram](img/data-migr-arch.png)

### Description ###


Environments
-------------

Obfuscation of sensitive information
-------------------------------------

Details on Processing files
-----------------------------

