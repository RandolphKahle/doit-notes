---
date: 2020-09-25T07:12
tags:
    - amazon/aws/
---

# aws-iam

## Key Concepts

IAM consists of *users*, *groups*, *roles*, and *policies*. 

### Policies

IAM uses [[aws-iam-policy-document]]s to give permissions for [[aws-iam-user]] / [[aws-iam-group]] / [[aws-iam-role]] to take actions within AWS.


### Users
End users - general people, members of an organization.

The *Root Account* is the account created when a person first establishes a ??billing account?? with AWS. It has "god mode". Highly recommended to use a [[high-quality-password]] and to use [[aws-iam-account-mfa]] multi-factor authentication.

### Groups

Collections of users.


### Roles

A role as "attached" *policies*.

One can "attach' a role to e.g. an [[aws-compute-ec2]] instance. This means the ec2 instance does not need a local copy of the secure keys. If such an instance is hacked, then the attackers could do anything allowed by the associated role(s) *but* they would not have access to the actual keys.

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

# Exam Tipes
Associating a role with an EC2 instance is more secure than storing the access key information on the instance. You coul still be hacked and have a bad actor use your account, but they would not have the keys.

[[[z:zettels?tag=amazon/aws/iam/]]]
