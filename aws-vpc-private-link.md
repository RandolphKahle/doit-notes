---
date: 2020-10-06T10:00
tags:
  - amazon/aws/vpc/
---

# aws-vpc-private-link

Supports the linkage of many *client* VPCs to a service VPC.
The alternatives are:
* Open the service to the internet
* Create N:1 VPC peering relationships.

Requires:
* Network Load Balancer on the service side
* Elastic Network Interface on the client side


