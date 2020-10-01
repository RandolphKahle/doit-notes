---
date: 2020-09-30T17:59
tags:
  - amazon/aws/storage/
---

# aws-ami

There are two types of AMI. 

## Dimensions

Region, operating system, architecture (32-bit, 64-bit, ARM), Launch permissions, root device storage (Instance store (EPHEMERAL) or [[aws-ebs]](EBS)) 

### EBS Volume
Root device is an EBS volume created from an EBS [[aws-ebs-snapshot]].

### Instance Store Volume
Root device is an instance store volume created from a template stored in an [[aws-s3-bucket]].