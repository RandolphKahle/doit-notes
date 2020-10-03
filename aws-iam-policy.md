---
date: 2020-10-03T08:13
tags:
    - amazon/aws/iam/
---

# aws-iam-policy

A policy is a JSON formated document that defines permissions. A policy much be *attached* to take effect.

* Identity policy -  [[aws-iam-user]], [[aws-iam-group]], [[aws-iam-role]] and define allowed actions.
* Resource policy - attached to a resource such as an [[aws-s3-bucket]] specifies who has access to the resource and what actions they can perform on that resource.

A policy is simply a list of statements in a JSON format
```
{
  "Version": "2012-10-17",
  "Statement" : [
    {},
    {},
    {}
  ]
}
```

Each statement represents an AWS API request, such as starting an [[aws-compute-ec2-instance]].

