---
date: 2020-09-25T07:12
tags:
    - amazon/aws/iam/
---

# Identity and Access Management (IAM)

## Key Concepts

IAM allows you to securely and accurately control access to AWS resource by users and groups.

IAM consists of *users*, *groups*, *roles*, and *policies*. 

### Users
End users - general people, members of an organization.
*Real* users can be associated with an IAM user through authentication.

End users must be *authenticated* before they use AWS resources.

Once authenticated, users must be *authorized* to use AWS services.
By default **no** permissions are granted to an IAM user ??or group??.
Permissions are granted through a policy.

The *Root Account* is the account created when a person first establishes a ??billing account?? with AWS. It has "god mode". Highly recommended to use a [[[high-quality-password]]] and to use [[aws-iam-account-mfa]] multi-factor authentication.

### Groups

Collections of users.
A group makes it easier to manage a set of permissions uniformly across multiple users.

### Roles

User can *assume* an IAM role after authenticated by a federated identity provider such as Facebook or Google.

A role as "attached" *policies*.

One can "attach' a role to e.g. an [[aws-compute-ec2]] instance. This means the ec2 instance does not need a local copy of the secure keys. If such an instance is hacked, then the attackers could do anything allowed by the associated role(s) *but* they would not have access to the actual keys.

### Policies

IAM uses [[aws-iam-policy-document]]s to give permissions for [[aws-iam-user]]s / [[aws-iam-group]]s / [[aws-iam-role]]s to take actions within AWS.

A policy document 


### Features
* Centralized control of AWS account
* Shared access to AWS account
* Granular Permissions
* Identity Federation (Active Directory, Facebook, LinkedIn, etc.)
* Multifactor Authentication
* Temporary access for users/devices
* Password rotation policy
* Integrates with AWS services
* PCI DSS Compliance

# Exam Tips
Associating a role with an EC2 instance is more secure than storing the access key information on the instance. You could still be hacked and have a bad actor use your account, but they would not have the keys.

### aws-iam


[[[z:zettels?tag=amazon/aws/iam/]]]
