#concept #module_4

A Security Group is a virtual firewall that controls inbound and outbound Internet traffic for a specific **[[Amazon Elastic Compute Cloud (EC2)]] instance**.

Just like [[Network Access Control List (ACL)]]s, they have rules that determine whether a packet is allowed / denied.

A security group is **stateful**, which means it **remembers previous outbound packet request and allows the same inbound packet to proceed regardless of security group rules**.

By default, a security group **denies all inbound and outbound traffic**.

A security group can be changed when an instance is stopped or running.