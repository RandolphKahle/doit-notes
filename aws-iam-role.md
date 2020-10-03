---
date: 2020-09-25T08:18
tags:
    - amazon/aws/iam/
---

# aws-iam-role

I'm still not entirely certain how to describe an AWS IAM *role*. 

It seems to be the link between a policy and ??

Example: A role "EC2 can access an S3 Bucket" would be an EC2 role associated with / bound to a policy show in the [[aws-iam-policy]] example.

"Trusted Entity" -> "Role" -> "Policy"...

? What are permission boundaries ?

? Can add tags ? - why? what do they do in this context?

"InLine Policy" is coded within the role definition. They say the "scope" of the policy is limited to the specific "role".

