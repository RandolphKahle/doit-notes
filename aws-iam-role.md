---
date: 2020-09-25T08:18
tags:
    - amazon/aws/iam/
---

# IAM Role

An AWS IAM role is an association between parties and permissions.

An **EC2 instance** can *write* to an **S3 bucket**.

So, *[[aws-arn]]* [[aws-iam-policy]] *[[aws-arn]]* ??


Example: A role "EC2 can access an S3 Bucket" would be an EC2 role associated with / bound to a policy show in the [[aws-iam-policy]] example.




Can add [[aws-iam-tags]] ? - why? what do they do in this context?

"InLine Policy" is coded within the role definition. They say the "scope" of the policy is limited to the specific "role".

### aws-iam-role