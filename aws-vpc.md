---
date: 2020-10-04T12:15
tags:
  - amazon/aws/
---

# aws-vpc

# Amazon Virtual Private Cloud. 

Allows you to build and launch resources in an isolated section of the AWS system.

## Concepts
* **Virtual Private Cloud** - virtual network dedicated to an [[aws-iam-account]].
* **Subnet** - A range of IP addresses in a VPC
* **Route Table** - Set of rules that determine where network traffic is directed.
* **Internet Gateway** - An attached gateway that allows communication with the Internet.
* **VPC Endpoint** - Supports private communication between a VPC and a supported AWS and VPC Endpoint services.

## Default VPC
* Easy to use - ready to deploy EC2
* Route out to Internet
* All instances have public and private IP addresses.

## Custom VPC

## VPC Peering
Connect to subnets.
Connect VPCs in different accounts or in the same account.
Star configuration. One central VPC and four attached VPCs.
There is *no* transitive peering. (what does that mean)

Can Peer between regions

Subnet *cannot* cross availability zones (unlike GCP where a subnet is a regional resource).

## Internet Gateway

## NAT Gateway

Network Address Translation - simply a way to provide isolation and a translation from private IP addresses and the public, routable IP addresses.

NAT *instances* are no longer recommended as they are singular instead of a shared, secure, resilient service. (However, NAT instances may still be on the exam).

