---
date: 2020-09-29T14:36
tags:
  - amazon/aws/storage/s3/
---

# aws-s3-performance


## Core operations

Performance is **per prefix**

PUT, COPY, POST, DELETE 3,500 operations per second per prefix

GET, HEAD 5,500 operations per second per prefix.

## KMS Limits

Each encrypt / decrypt takes extra processing power. 

Regions specific limits. Either 5,500, 10,000, or 30,000 request per second with MKS.

## Multi-Part Uploads

100MB++ recommended  
5GB++ required  

## Byte Range Download

Parallel download or part of object download (such as fetching header)