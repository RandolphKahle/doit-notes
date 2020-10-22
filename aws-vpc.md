---
date: 2020-10-04T12:15
tags:
  - amazon/aws/
---

# Amazon Virtual Private Cloud. 

Allows you to build and launch resources in an isolated section of the AWS system.

## Concepts
* **Virtual Private Cloud** - virtual network dedicated to an [[aws-account]]. It uses a single IP address [[network-subnet-cidr]].
* **Subnet** - A range of IP addresses within the containing VPC [[network-subnet-cidr]].
* **Route Table** - Set of rules that determine where network traffic is directed.
* **Internet Gateway** - A gateway attached to the VPC that allows communication with the Internet.
* **VPC Endpoint** - Supports private communication between a VPC and a supported AWS and VPC Endpoint services.

## Default VPC
* Easy to use - ready to deploy EC2
* Route out to Internet
* All instances have public and private IP addresses.
* NACL?
* Security Group?

## Custom VPC
* No subnets allocated
* Default route table (all traffic goes to VPC CIDR block)
* Default NACL (allows everything)
* Default Security Group (allows everything)

## VPC Peering
Connect to subnets.
Connect VPCs in different accounts or in the same account.
Star configuration. One central VPC and four attached VPCs.
There is *no* transitive peering. (what does that mean)

Can Peer between regions

## Subnet

Subnet *cannot* cross availability zones (unlike GCP where a subnet is a regional resource).

## VPN

An [[[network-protocol-ipsec]]] link between an external network and a VPC. Requires a hardware device or software appliance in the external network and a VPN [[aws-vpc-virtual-private-gateway]] on the AWS side.


## Internet Gateway

## Security Group
A security group is tied to a VPC.

### aws-vpc

[[[z:zettels?tag=amazon/aws/vpc/*]]]