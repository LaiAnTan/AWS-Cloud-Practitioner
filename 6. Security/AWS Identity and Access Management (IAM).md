#service #module_6

A service to manage AWS services and resources securely.

There are many features of IAM that can be used to configure access based on a company’s specific operational and security needs:

### AWS Account Root User

The root user has complete access to all AWS services and resources in the account.

The best practice is to not use the root user for everyday tasks.

### IAM Users

An IAM User can be created that consists of a name and credentials.

It represents the person or application that interacts with AWS services and resources.

By default, IAM users have no permissions, and necessary permissions must be granted.

The best practice is to create an IAM user for each person that needs to access AWS services and resources.

### IAM Policies

An IAM Policy is a **JSON document that describes what API calls a user can / cannot make**. 

For example:
```
{
	"Version": 2012-10-17,
	"Statement": {
		"Effect": "Allow",
		"Action": "s3:ListObject",
		"Resource": "arn:aws:s3:::AWSDOC-EXAMPLE-BUCKET"
	}
}
```

The above means that the policy states that any user or group with this policy attached can make the`s3:ListObject` API call on the resource `arn:aws:s3:::AWSDOC-EXAMPLE-BUCKET`.

IAM Policies can be attached to IAM Users or IAM Groups.

The best practice is to follow the **principle of least privilege** when granting permissions, which states to only grant necessary permissions and no more.

### IAM Groups

IAM Groups are collections of IAM Users.

When an IAM Policy is assigned to a group, all users in the group are granted permissions specified by said policy.

It is easier to manage user policies with groups.
### IAM Roles

IAM Roles are **temporary** identities that can be granted to allow temporary access to AWS services and resources.

IAM Roles can be given to users, external identities, applications, or other AWS Services.

When an identity assumes a role, it **abandons all previous permissions** that it has and assumes the permissions of said role.

### Multi Factor Authentications (MFA)

Multi Factor Authentication provides an extra layer of security to an AWS Account by requesting a second form of authentication after the password, such as a code sent to a phone.
