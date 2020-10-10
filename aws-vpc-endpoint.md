---
date: 2020-10-05T17:56
tags:
  - amazon/aws/vpc/
---

# VPC Endpoint


A VPC endpoint is a horizontally scaled, redundant, and highly available IP communication port. They may be associated
with various services such as [[aws-vpc-private-link]].

There are two types of VPC endpoints:
* [Interface Endpoint](aws-vpc-interface-endpoint)
* Gateway Endpoints


## Gateway Endpoint

Appear as if they are a [[network-nat]] endpoint. Currently supported:
* Amazon S3
* DynamoDB

### aws-vpc-endpoint