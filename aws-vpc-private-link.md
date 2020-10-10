---
date: 2020-10-06T10:00
tags:
  - amazon/aws/vpc/
---

# Private Link

PrivateLink provides a private connection between VPCs
and:
* AWS services
* AWS Marketplace applications
* ?Your own VPCs?
* On-premise services

by providing a private [endpoint](aws-vpc-endpoint).

Eliminates the need for an [Internet Gateway](aws-vpc-internet-gateway), [NAT device](aws-vpc-gateway-nat), or a public IP address.

Also works with [Direct Connect](aws-vpc-direct-connect) to support a private connection to services on-premise.

![Private Link](./static/privatelink_overview.jpg)

## Client side

An *Interface Endpoint* is created in a specific VPC. The interface endpoint ??has the name of the remote 'service' associated with it??

Within a subnet an *endpoint network interface* presents a private IP address that allows network traffic to flow to the remote service.

Security groups may be associated with the endpoint network
interface.

In some situations (AWS services and AWS Marketplace Partner services) a private DNS for the endpoint can be enabled.

Supports the linkage of many *client* VPCs to a service VPC.
The alternatives are:
* Open the service to the internet
* Create N:1 VPC peering relationships.

Requires:
* Network Load Balancer on the service side
* Elastic Network Interface on the client side

 # Exam Tips
 
 Connect VPC to tens, hundreds, or thousands of customer VPC then think about Private Link.

### aws-vpc-private-link