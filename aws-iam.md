---
date: 2020-09-25T07:12
tags:
    - amazon/aws/security
---

# aws-iam

## Key Concepts

### Users
End users - general people, members of an organization.

?? Root Account: The identity of the user who created the AWS account. It has "god mode". Want to have [[aws-iam-account-mfa]] multi-factor authentication.

### Groups

Collections of users

### Policies

Uses [[aws-iam-policy-document]]s to give permissions for [[aws-iam-user]] / [[aws-iam-group]] / [[aws-iam-role]] to take actions within AWS.

### Roles

?? Not clear yet how to describe this ??

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

[[[z:zettels?tag=amazon/aws/iam/*]]]
