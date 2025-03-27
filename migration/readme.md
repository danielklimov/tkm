Migration Plan
===============

Approach
---------

To implement migration along the same design patterns as used for
implementation of Data Warehouses.

### Assumptions ###

There are 2 kinds of data that must be migrated:

1. Database tables in 2 PostgreSQL databases - QVP and SVP.
2. Files in OCI object storage for QVP and SVP.

Target storage:

1. 1 PostgreSQL database - Uni PACC.
2. OCI object storage for files.

### Incremental Loads ###

Data are going to be moved in two phases:

1. Bulk migration - all data from all tables, all files.
2. Incremental migration - periodical extraction of new/changed data
   from source tables and from OCI object storage.

The approach outlined above allows to make the transition
Unified PACC smooth, provides room for error during every step of migration,
reduces the load on source databases.

### Cutover Plan ###

After successful bulk migration and several incremental migrations, 
a set of test queries are run on source and target systems to ensure that
all data have been copied, certain key indicators match on the source and the target.
Uni PACC application is tested on prod environment with several test user accounts
to make sure there are no errors in foreign keys, semantics of the data model is not
damaged after migration, all files are in place.

When there are no more errors, the source applications are switched off,
the last incremental load is executed and the target system goes into live production.

### Data Layers ###

Tools
------

Data Integration Architecture
------------------------------

### Diagram ###

![Migration Architecture Diagram](img/data-migr-arch.png)

### Description ###


Environments
-------------


