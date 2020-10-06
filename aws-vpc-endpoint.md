---
date: 2020-10-05T17:56
tags:
  - amazon/aws/vpc/
---

# aws-vpc-endpoint
# VPC Endpoint


A VPC endpoint provides a private connection between a VPC
and (supported) AWS service. 
It is powered by *PrivateLink* without requiring an
internet [[aws-gateway]], [[network-nat]] device, VPN connection, or AwS
Direct Connect connection.

Instances on the VPC can use internal, private IP addresses.
All traffic is on the Amazon network.

Endpoints are virtual and can be horizontally scaled, redundant, and HA.

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

