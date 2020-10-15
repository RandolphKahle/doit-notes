---
date: 2020-10-15T08:14
tags:
  - amazon/aws/
---

# Key Management Service

* Regional
* Manages encryption keys
* CMK (Customer Master Key). 
  * AWS Managed (free)
  * AWS Owned (typically hidden)
  * Customer Managed
* Keys never leaves Region. 
* Pointer to information. 
* 4KB in size
* FIPS 140-2 Level 2

Symmetric Key
* AES-256
* Master key for data encryption
* Faster

Asymmetric Key
* Public / Private
* RSA or Elliptic-curve (ECC)
* Sign messages and verify signatures

Example
```
{
  "Sid": "Enable IAM User Permissions",
  "Effect": "Allow",
  "Principal": {"AWS": "arn:aws:iam:1112323212322:root"},
  "Action": "kms:*",
  "Resource": "*"
}
```


### aws-kms