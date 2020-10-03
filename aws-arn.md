---
date: 2020-10-03T08:13
tags:
    - amazon/aws/
---

# aws-arn

Amazon Resource Name (ARN) - uniquely identifies *any* resource within AWS.

Syntax:

```
arn:partition:service:region:account_id:
```

* **arn** - URI scheme  
* **partition** - segregates totally different infrastructures. Currenly *aws* and *aws-cn* for China.
* **service** - specific AWS service such as s3, rds, e tc.
* **region** - geographic region
* **account_id** - twelve digit account identifier

ends with:

* resource
* resource_type/resource/qualifier
* resource_type/resource:qualifier
* resource_type:resource
* resource_type:resource:qualifier

Examples

arn:aws:iam::123456789012:user/mark

arn:aws:s3:::my_awesome_bucket/image.png

arn:aws:dynamodb:us-east-1:123456789012:table/orders

arn:aws:ec2:us-east-1:123456789012:instance/*

