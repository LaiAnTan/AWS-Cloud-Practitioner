#service #module_6

A service to **consolidate and manage multiple AWS accounts within a central location**.

When an organisation is created, a **root** is automatically created, which acts as the parent container for all accounts in the organisation.

**Service Control Policies (SCPs)** are used to control permissions of accounts in the organisation.

### Organisational Unit (OU)

Accounts in an organisation can be further grouped into groups called **Organisational Units**.

This makes it easier to manage accounts with similar business or security requirements.

Workloads or applications with specific security requirements can be isolated by using Organisational Units in combination with [[AWS Identity and Access Management (IAM)#IAM Policies|IAM Policies]].
