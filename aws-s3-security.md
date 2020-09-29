---
date: 2020-09-29T13:42
tags:
  - amazon/aws/storage/s3/
---

# aws-s3-security

By default, all newly created buckets are set to **deny public access**.

Bucket Policy

Access Control List

Access logs sent to another bucket–even in a different account.

## Encryption

### In transit

SSL/TLS (which versions?)

### At rest

* Server side
  * S3 Managed Keys **SSE-S3** (AWS does all key management)
  * S3 Key Management Service managed keys **SSE-KMS**
  * S3 Server side encryption with customer supplied keys **SSE-C**

* Client side