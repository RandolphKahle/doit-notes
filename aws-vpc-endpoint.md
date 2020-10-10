---
date: 2020-10-05T17:56
tags:
  - amazon/aws/vpc/
---

# VPC Endpoint


A VPC endpoint is a horizontally scaled, redundant, and highly available IP communication port. They may be associated
with various services such as [[aws-vpc-private-link]].


## Interface Endoint

An elastic network interface with a private IP address that
serves as an entry point for traffic destined to a supported service.

* Amazon API Gateway
* AWS CloudFormation
* Amazon CloudWatch
* Amazon CloudWatch Events
* Amazon CloudWatch Logs
* AWS Code Build
* AWS Config
* Amazon EC2 API
* Elastic Load Balancing API
* AWS Key Management Service
* Amazon Kinesis Data Streams
* Amazon SageMaker and Amazon SageMaker Runtime
* Amazon SageMaker Notebook Instance
* AWS Secrets Manager
* AWS Security Token Service
* AWS Service Catalog
* Amazon SNS
* Amazon SQS
* AWS Systems Manager
* Endpoint services hosted by other AWS accounts
* Supported AWS Marketplace partner services


## Gateway Endpoint

Appear as if they are a [[network-nat]] endpoint. Currently supported:
* Amazon S3
* DynamoDB

### aws-vpc-endpoint