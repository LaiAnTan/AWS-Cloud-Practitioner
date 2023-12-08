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

> [!example] Definitions
> Default Tenancy: Multiple AWS customers on one host
> Dedicated Tenancy: Only one AWS customer on a particular host

2. Convertible Reserve Instances
	Used when EC2 instances need to run in different Availability Zones or different EC2 Instance types are required (i.e. more flexibility in running EC2 instances)
	
	Trade off: a smaller discount.

Three types of payment options:
- Full upfront
- Partial upfront
- No upfront

### Savings Plans
Reduced  [[#On - Demand]] rates (up to 72%) when committing to an instance family and region for a 1-year or 3-year term.

**No need to specify EC2 instance type, size, OS and tenancy**.

No capacity reservation.

### Spot Instances

Reduced [[#On - Demand]] rates (up to 90%)

Trade off: **instance may be interrupted if capacity is no longer available**.

Suitable for workloads:
- with flexible start / end time
- that can be interrupted

### Dedicated hosts

Physical servers fully dedicated to a singular customer.

Suitable for **maintaining license compliance**.

Most expensive.

