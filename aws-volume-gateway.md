---
date: 2020-09-29T18:12
tags:
  - amazon/aws/storage/gateway/
---

# aws-volume-gateway

Provides an iSCSI endpoint for local attachment use.


## Stored Volumes

All data is available locally with low-latency. Provides durable 1TB to 16TB. Async backed up in the form of EBS snapshots.

## Cache Volumes

Keeps the most frequently used (blocks of) data locally. From 1GB to 32TiB and attach as iSCSI devices. Data is stored in S3. 

The backing is sent to Amazon and is stored in an S3 bucket as an object store.

