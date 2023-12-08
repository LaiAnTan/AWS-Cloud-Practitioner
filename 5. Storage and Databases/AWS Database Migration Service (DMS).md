#service #module_5

A service to **migrate** relational / non relational database or other types of data stores

DMS moves data between a source and target database.

There are two types of database migration:
- **Homogeneous** migration: source and target database have **same** type
- **Heterogeneous** migration: source and target database have **different** types

To perform a heterogenous migration, the source schema and code is converted using [[AWS Schema Conversion Tool]], then DMS is used to migrate the data.

Other uses of DMS include:
- Development and test database migrations: test applications against production data without affecting production users
- Database consolidation: combining databases into a single database
- Continuous replication: send ongoing copies of data to other target sources
