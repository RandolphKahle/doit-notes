---
date: 2020-10-03T08:13
tags:
    - amazon/aws/iam/
---

# IAM Policy

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

Each statement represents an AWS API request, such as starting an [[aws-compute-ec2]] instance.

```
{
	"Version": "2012-10-17",
	"Statement" : [
		{
 		"Sid" : "SpecificTable",
 		"Effect": "Allow",
 		"Action": [
 			"dynamodb:BatchGet*",
 			"dynamodb:DescribeStream",
 			"dynamodb:DescribeTable",
 			"dynamodb:Get*",
 			"dynamodb:Query",
 			"dynamodb:Scan",
 			"dynamodb:BatchWrite*",
 			"dynamodb:CreateTable",
 			"dynamodb:Delete*",
 			"dynamodb:Update*",
 			"dynamodb:PutItem",
 		],
 		"Resource": "arn:aws:"dynamodb":*:*:table/MyTable"
		}
	]
}
```

# Exam Tips

* Permission are denied unless allowed.
* Explicit deny overrides anything in any other policy.
* Policy does not do anything unless attached to a user, group, or role.
* If there are multiple policies, AWS will UNION all policies.
* AWS managed policies and Customer managed policies

## Permission Boundaries

Used to set an upper limit on permissions granted by a delegatee?

For example, a user is granted full rights to all of AWS... A super user... Then set a permission boundary to limit to administration of DynamoDB. Then the only things this user can do are the
administrative functions related to DynamoDB.

### aws-iam-policy

