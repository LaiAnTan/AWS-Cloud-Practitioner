#concept #module_4

Subnets are **sections of a [[Amazon Virtual Private Cloud (VPC)]]** in which resources can be grouped based on security or operational needs.

There are two types of subnets:

1. **Public subnets** contain resources that need to be accessed by the public.

2. **Private subnets** contain resources that should only be accessible through a private network.

By partitioning a VPC into subnets, customers are only allowed to interact with what is meant for them, and prevents them from accessing restricted resources.

Every subnet has an [[Network Access Control List (ACL)]] for security purposes.