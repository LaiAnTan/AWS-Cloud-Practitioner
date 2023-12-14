---
~
---
#service #extra 

A cloud - based **hardware security module** (HSM) that enables customers to easily generate and use encryption keys in AWS.

There are key differences between AWS CloudHSM and [[AWS Key Management Service (KMS)]] although they are similar.

- CloudHSM is single tenant (only belongs to one customer), while KMS is multitenant (KMS uses HSM's internally, but not exclusive to one customer)
- CloudHSM is more compliant than KMS, CloudHSM meeting stricter security standards.

Use cases for AWS CloudHSM include:

- Encrypting data at rest
- Offloading SSL processing for web servers
- Protect private keys for an issuing certificate authority