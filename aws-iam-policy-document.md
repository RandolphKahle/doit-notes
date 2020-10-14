---
date: 2020-09-25T08:13
tags:
    - amazon/aws/iam/
---

# IAM Policy Document

Technical

JSON formatted gives permissions to [[aws-iam-user]] / [[aws-iam-group]] / [[aws-iam-role]] describing what they are allowed to do.

JSON formatted document. The following grants all rights
to all resource, also know as the administrator!

```
{
  "Version": "2020-09-25",
  "Statement": [
    {
      "Effect": "Allow",
      "Action": "*",
      "Resource": "*"
    }
  ]
}
```
### aws-iam-policy-document
