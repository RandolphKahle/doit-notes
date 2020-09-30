---
date: 2020-09-25T06:51
tags:
    - amazon/aws/storage/
---

# aws-ebs
 
# Elastic Block Storage

Block storage attached to a single EC2 instance (VM) and formatted to function as a file system.
The EBS volume must be in the same availability zone as the associated EC2 instance.


## Types

| API | Description | Size | IOPS |
| ----------- | ----------- |  ----------- | ----------- |
| **gp2** | General purpose SSD | 1G to 16T | 16000 |
| **io1** | High-performance SSD | 4G to 16T | 64000 |
| **st1** | Low cost, frequent access, high-through put. Big Data & Data Warehouse | 500G to 16T | 500 |
| **sc1** | Low cost for file server | 500G to 16T | 250 |
| **Standard**| Previous generation. Seldom used data | 1G to 1T | 40 to 200 |

## Tasks

### Move an EC2 instance
To move an EC2 instance to another availability zone:
* Create a snapshot of the boot disk
* Create a private image (AMI) from the snapshot
* Create a new EC2 instance

If you need to move to a different region, you must first move the AMI to the destination region. Once moved, create a new EC2 instance.

