#concept #extra

Multiple **interdependent** [[Amazon Elastic Compute Cloud (EC2)]] instances can be launched into a placement group to influence their placement according to three placement strategies as follows:

### Cluster Placement Group

A logical grouping of instances within a singular [[AWS Availability Zones|Availability Zone]].

![[cluster placement group.png]]

### Partition Placement Group

Each EC2 group is divided into logical segments called partitions, where each partition has its own set of racks.

This helps reduce the likelihood of correlated hardware failures.

![[partition placement group.png]]
### Spread Placement Group

A group of instances that are each placed on distinct hardware.

Spread placement groups are recommended for applications that have a **small number of critical instances that should be kept separate from each other**.

![[spread placement group.png]]
