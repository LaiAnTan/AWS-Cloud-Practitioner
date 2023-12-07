#concept  #module_2

There are five pricing options for [[Amazon Elastic Compute Cloud (EC2)|EC2 Instances]]:

### On - Demand
Suitable for **short - term, irregular** workloads.
**No upfront costs / contracts**.
Only pay for the compute time that was used.

### Reserved Instances
A discount that is applied to [[#On - Demand]] Instances when **committing to a 1-year or 3-year term**.

Two types of reserved instances:

1. Standard Reserve Instances
	Must specify:
	- [[EC2 Instances Types|Instance Type]]
	- Instance Size
	- Platform Description (OS)
	- Tenancy (default / dedicated)
	Can specify:
	- [[AWS Availability Zones]] to reserve EC2 capacity

2. Convertible Reserve Instances
	Used when different AZ