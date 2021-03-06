---
date: 2020-10-08T11:11
tags:
  - amazon/aws/vpc/gateway/
---

# Internet Gateway


An AWS VPC Internet Gateway is a horizontally scalable, redundant, and highly available connection service.

This is a bi-directional interface. **If a subnet has an associated route to the Internet Gateway then it *is* a public subnet**.

## Major Functions
* Provides a *route table target* for internet-bound traffic
* Performs NAT for instances with a *public* IP address

(Does *not* perform NAT for instances with only a private IP address)



### aws-vpc-internet-gateway
