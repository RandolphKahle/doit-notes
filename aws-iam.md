---
date: 2020-09-25T07:12
tags:
    - amazon/aws/security/iam
---

# aws-iam

## Key Concepts

### Users
End users - general people, members of an organization

### Groups

Collections of users

### Policies

Made of [[aws-iam-policy-document]]s "Policy Documents".
Formatted in JSON.
Give permissions for User/Group/Role to take actions within AWS.

### Roles

?? Not clear yet how to describe this ??

Features:
* Centralized control of AWS account
* Shared access to AWS account
* Granular Permissions
* Identity Federation (Active Directory, Facebook, LinkedIn, etc.)
* Multifactor Authentication
* Temporary access for users/devices
* Password rotation policy
* Integrates with AWS services
* PCI DSS Compliance

