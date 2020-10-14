---
date: 2020-09-25T06:52
tags:
    - amazon/aws/storage/
---

# aws-s3

S3 Storage bucket system.

## Technical

### Architecture Essentials
* Key
* Value
* Version ID
* Metadata
* Sub-resources
  * Access control list
  * Torrent

### Data consistency
* Read-after-write for PUTs of new objects
* Eventual consistency for overwrite-PUTs and DELETEs

For example, if you upload version 1 of a file and then overwrite with version 2, it will take some time before you get version 2 on a fetch.

* 99.9% available (SLA)
* 99.99% availability (Build-To specification)
* 99.999999999% durability


### Storage Tiers


| Tier | Durability | Availability SLA | Design-to | Notes |
| --- | ---: | ---: | ---: | --- |
| S3 Standard | 99.999999999% | 99.9% | 99.99% | 2 facility loss |
| S3 Intelligent Tiering | 99.999999999% | 99% | 99.9% |2 facility loss |
| S3 Infrequent Access  | 99.999999999% | 99% |99.9% | 2 facility loss|
| S3 One Zone | 99.999999999%  | 99% |99.5% | Uses only 1 zone|
| S3 Glacier | 99.999999999% | N/A| N/A| 2 facility loss|
| S3 Glacier Deep Archive | 99.999999999% |N/A |N/A | 2 facility loss|


#### S3 Standard


| Storage | Price |
| --- | ----------- |
| < 50 TB | 0.0230 |
| < 450 TB  | 0.0220 |
| > 500 TB | 0.0210 |


#### S3 Intelligent Tiering
 Storage | Frequent Access | Infrequent Access | Management |
| --- | ----------- | --- |  -- |
| < 50 TB | 0.0230 |
| < 450 TB  | 0.0220 |
| > 500 TB | 0.0210 |
| Infrequent Access Tier |  | 0.0125 |
| Management | | | 0.2500 per 1,000 objects |



#### S3 Standard Infrequent Access
| Storage | Price |
| --- | ----------- |
| All | 0.0125 |


#### S3 One Zone Infrequent Access

| Storage | Price |
| --- | ----------- |
| All | 0.0100 |

#### Glacier
For 1 minute to 12 hours

| Storage | Price |
| --- | ----------- |
| All | 0.0040 |


#### Glacier Deep Archive
12 Hour retrieval (probably in a tape vault)
| Storage | Price |
| --- | ----------- |
| All | 0.00099 |



### Other
* Lifecycle Management
* Versioning
* Can encrypt
* MFA (for deletion)
* Secure with ACL and bucket policies

## Pricing
* Storage
* Requests (operations)
* Tier policy
* Data transfer
* Transfer acceleration. For in-coming files, once they hit an Amazon edge location the file is transferred using Amazon's backbone network. (Huh? Isn't this what Google does automatically?)
* Cross Region Replication

## Tags (metadata)

Object tags are a tool you can use to enable simple management of your S3 storage. With the ability to create, update, and delete tags at any time during the lifetime of your object, your storage can adapt to the needs of your business. These tags allow you to control access to objects tagged with specific key-value pairs, allowing you to further secure confidential data for only a select group or user. Object tags can also be used to label objects that belong to a specific project or business unit, which could be used in conjunction with S3 Lifecycle policies to manage transitions to other storage classes (S3 Standard-IA, S3 One Zone-IA, and S3 Glacier) or with S3 Replication to selectively replicate data between AWS Regions.



# Exam Tips
* S3 is **Object Based**. Not block storage.
* Size is 0 to 5TB
* Unlimited storage
* Files stored in buckets (with unique global names. default to Virginia, otherwise, region in DNS name)
* Return code for a successful upload is an HTTP 200 status code
* MFA for deletes is available
* Each object
  * Key
  * Value
  * Version ID
  * Metadata
  * Sub-resources
    * Access Control List (ACL) (bucket or object)
    * Torrent
  * Consistency
    * Read-After-Write for initial PUT
    * Eventual-Consistency for update PUT or DELETE
  * Storage Classes
    * S3 Standard
    * S3 Infrequent Access
    * S3 Infrequent Access One Zone
    * S3 Intelligent Tiering
  * Glacier
  * Glacier Deep Archive (12 hour retrieval time)
  * S3 FAQ!!!

[[[z:zettels?tag=amazon/aws/storage/s3/*]]]