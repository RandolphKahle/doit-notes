---
date: 2020-10-05T17:56
tags:
  - amazon/aws/vpc/
---

# aws-vpc-endpoint

A VPC endpoint provides a private connection between a VPC
and (supported) AWS service. 
It is powered by *PrivateLink* without requiring an
internet [[aws-gateway]], NAT device, VPN connection, or AwS
Direct Connect connection.

Instances on the VPC can use internal, private IP addresses.
All traffic is on the Amazon network.

Endpoints are virtual and can be horizontally scaled, redundant, and HA.