---
date: 2020-09-29T18:12
tags:
  - amazon/aws/storage/volume-gateway/
---

# aws-volume-gateway

Run an on-premise VM that connects to Amazon. This can provide an NFS or SMB file share point, an iSCSI block storage endpoing, or ??

## NFS / SMB

Files are backed up on Amazon S3.

## iSCSI

Stored volume - locally all data is available with low-latency. Provides durable 1TB to 16TB. Async backed up in the form of EBS snapshots.



The backing is sent to Amazon and is stored in an S3 bucket as an object store.

