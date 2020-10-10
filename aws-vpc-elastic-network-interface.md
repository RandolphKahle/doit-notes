---
date: 2020-10-10T14:03
tags:
  - amazon/aws/vpc/
---

# Elastic Network Interface

A *logical* networking component in a VPC that
represents a virtual network card.
Can include:
* A primary private IPv4 address for the subnet CIDR block
* One or more secondary private IPv4 addresses
* One [Elastic IP Address](aws-vpc-elastic-ip-address) (IPv4) per private IPv4 address
* One public IPv4 address
* One or more IPv6 addresses
* One or more security groups (is there an upper limit?)
* A MAC address
* A source/destination check flag
* A description

This type of network interface is an independent entity. 
It can be attached, removed, and re-attached to
different instances while maintaining its independent
attributes.
The security groups, IP address, etc. can be changed 
and those change remain with the interface object.

A VPC flow log may be associated with the interface.


### aws-vpc-elastic-network-interface
