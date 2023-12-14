#concept #extra

An S3 Lifecycle Configuration is an XML file that consists of a set of predefined rules with predefined actions that [[Amazon Simple Storage Service (S3)]] performs on objects during their lifetimes.

There are two types of actions:

### Transition Actions

These actions when objects transition to another storage class.

Possible use cases are to transition objects to a lower [[S3 Storage Classes|storage class]] when they are no longer frequently accessed.

### Expiration Actions

These actions define when objects expire.

S3 automatically deletes expired objects.