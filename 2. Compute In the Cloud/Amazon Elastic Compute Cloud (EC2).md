#service #module_2

Amazon calls virtual servers **Elastic Compute Cloud (EC2)**.

One server is referred to as an **EC2 instance**.

There are many EC2 instances (virtual machines) running on a singular host machine (multitenancy).

> [!tip] Multitenancy: The sharing of underlying hardware.

A **hypervisor** on the host machine is responsible for isolating the virtual machines as they share resources, maintaining security.

>[!info] One EC2 instance is not aware of any other instances on the same host.
