#concept #module_5

There are eight types of S3 Storage Classes:

### S3 Standard
- Suitable for frequently accessed data
- Stores data in a **minimum of 3 [[AWS Availability Zones]]**.
- 11 nines of durability (i.e. there is a 99.999999999% probability the data will be intact after 1 year)

### S3 Standard - Infrequent Access (S3 Standard - IA)
- Suitable for infrequently accessed data
- Similar to S3 but with a **lower storage price** and **higher retrieval price**

### S3 One Zone - Infrequent Access (S3 One Zone - IA)
- Stores data in a single [[AWS Availability Zones|Availability Zone]].
- Lower price than S3 Standard - IA

### S3 Intelligent Tiering
- Suitable for data with **unknown / changing access patterns**
- S3 Intelligent Tiering monitors object's access patterns and changes the storage class accordingly.
	1. `If data has not been accessed for 30 consecutive days, it is moved to S3 Standard-IA`
	2. `If data has been accessed in S3 Standard-IA, it is moved to S3 Standard`
- There will be a small monthly monitoring and automation fee per object

### S3 Glacier Instant Retrieval
- Suitable for archived data that requires immediate access.
- Object retrieval within a few milliseconds.

### S3 Glacier Flexible Retrieval
- Low cost storage for data archives.
- Object retrieval within a few minutes to hours (1 min - 12 hr)

### S3 Glacier Deep Archive
- Lowest-cost storage class for data archives.
- Object retrieval within 12 hours (12 hr - 48 hr)

### S3 Outposts
- Suitable for workloads with local data residency requirements that must satisfy demanding performance needs by keeping data close to on-premises applications.
- On premises [[Types of Storage Solutions#Object - level storage|object storage]] at AWS Outposts environment.
- Easier to retrieve, store, access data on AWS Outposts