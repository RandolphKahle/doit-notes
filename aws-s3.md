---
date: 2020-09-25T06:52
tags:
    - amazon/aws/storage/
---

# aws-s3

S3 Storage bucket system.

## Technical

An object has
* Key
* Value
* Version ID
* Metadata
* Sub-resources
  * Access control list
  * Torrent

Data consistency
* Read-after-write for PUTs of new objects
* Eventual consistency for overwrite-PUTs and DELETEs

For example, if you upload version 1 of a file and then overwrite with version 2, it will take some time before you get version 2 on a fetch.

* 99.9% available (SLA)
* 99.99% availability (Build to specification)
* 99.999999999% durability

asdf

* Storage Tiers
  * S3 Standard. Multiple devices in multiple facilities. Designed to survive the loss of two facilities concurrently.
  * S3-IA. S3 Infrequent Access. Less expensive, fast access, access charge.
  * S3 One Zone - IA. (Yikes!)
  * S3 Intelligent Tiering. 
  * S3 Glacier. Retrieval time configurable from minutes to hours.
  * S3 Glacier Deep Archive. Lowest cost. 12-hour retrieval (probably tape in a vault!)
* Lifecycle Management
* Versioning
* Can encrypt
* MFA (for deletion)
* Secure with ACL and bucket policies

Pricing
* Storage
* Requests (operations)
* Tier policy
* Data transfer
* Transfer acceleration
* Cross Region Replication
