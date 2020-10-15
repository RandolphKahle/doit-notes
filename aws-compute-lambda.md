---
date: 2020-10-15T09:59
tags:
  - amazon/aws/compute/
---
# Lambda

Serverless execution of code.

* Event triggers to run code
  * S3 bucket change
  * DynamoDB data change
* HTTP request
* Languages
  * Node.js
  * Java
  * Python
  * C#
  * Go
  * PowerShell

## Pricing
* Requests
  * First 1M free
  * Subsequent 1M $0.20
* Duration
  * $0.x per GB-second
  
## Triggers that call Lambda
* API Gateway
* AWS IoT
* Application Load Balancer
* CloudWatch events
* CloudWatch Logs
* Code Commit
* Cognito Sync Trigger
* DynamoDB
* Kinesis
* S3 
* SNS
* SQS

## Services that Lambda can call
* Aurora Servless
* DynamoDB
* API Gateway
* S3
* Lambda functions!

## x-ray

Helps debug serverless applications


### aws-compute-lambda