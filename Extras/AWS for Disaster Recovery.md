#concept #extra 

There are a few disaster recovery methods:
### Backup & Restore
Restoring a backup of a previously saved version of an application

### Pilot light
Data from one [[AWS Regions|Region]] to another is replicated and a copy of the core workload infrastructure is provisioned. 
Resources required to support data replication and backup, such as databases and object storage, are always on.
Other elements, such as application servers, are loaded with application code and configurations, but are "switched off" and are only used during testing or when disaster recovery failover is invoked.

### Warm Standby
A scaled down, but fully functional, copy of your production environment in another Region.

### Multi Site
The workload is run simultaneously in multiple Regions.

---

The spectrum of disaster recovery methods are shown below.

![[disaster recovery methods.png]]

Moving towards the right, application downtime decreases when using the methods shown.
