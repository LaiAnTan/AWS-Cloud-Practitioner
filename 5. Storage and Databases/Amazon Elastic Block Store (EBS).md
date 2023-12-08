#service #module_5

**[[Types of Storage Solutions#Block - level storage|Block - level storage]]** service where **data will persist** even after an [[Amazon Elastic Compute Cloud (EC2)]] instance is terminated.

**EBS Volumes** are created by defining the configuration (volume size, type), provisioning it and attaching it to an EC2 instance.

**Incremental Backups** called **EBS Snapshots** can also be created, where the first snapshot copies all the data, and subsequent snapshots only saves blocks of data **that have changed**.

EBS stores data in a single [[AWS Availability Zones|Availability Zone]], and the EC2 instance and EBS Volume must be in the same Availability Zone.
