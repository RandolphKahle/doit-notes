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

A more restrictive policy document:
```
"Sid" : "Stmt1505076701000",
"Effect": "Allow",
"Action" : [
   "s3:DeleteObject",
   "s3:GetObject"
   ],
"Condition": {
  "IpAddress": {
      "aws:SourceIP": "10.14.8.0/24"
      }
    },
"Resource": [
    "arn:aws:s3:::billing-marketing",
    "arn:aws:s3:::billing-sales"
]
```

* Sid - Who or What is authorized (**user**, **group**, **resource**)
* Action - Which tasks are allowed
* Condition - Which conditions need to be met for authorization
* Resource - Resource to which authorized tasks are performed.
### aws-iam-policy-document
