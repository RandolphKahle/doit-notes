---
date: 2020-09-29T11:18
tags:
  - amazon/aws/storage/s3/
---


# S3 One-Zone Infrequent Access (S3 One-Zone IA)


20% less than Standard IA

Customer must be prepared for data loss. 

Good for secondary backups (onpremise, other regions using Cross-Region-Replication)

**Not resilient to one-zone destruction**



Durability: 99.999999999%  
Availability: 99%

According to Amazon:

S3 One Zone-IA storage class is an Amazon S3 storage class that customers can choose to store objects in a single availability zone. S3 One Zone-IA storage redundantly stores data within that single Availability Zone to deliver storage at 20% less cost than geographically redundant S3 Standard-IA storage, which stores data redundantly across multiple geographically separate Availability Zones.

S3 One Zone-IA offers a 99% available SLA and is also designed for eleven 9’s of durability within the Availability Zone. But, unlike the S3 Standard and S3 Standard-IA storage classes, data stored in the S3 One Zone-IA storage class will be lost in the event of Availability Zone destruction.

S3 One Zone-IA storage offers the same Amazon S3 features as S3 Standard and S3 Standard-IA and is used through the Amazon S3 API, CLI and console. S3 One Zone-IA storage class is set at the object level and can exist in the same bucket as S3 Standard and S3 Standard-IA storage classes. You can use S3 Lifecycle policies to automatically transition objects between storage classes without any application changes.

### aws-s3-standard-infrequent-access-single-zone
