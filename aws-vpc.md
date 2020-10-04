---
date: 2020-10-04T12:15
tags:
  - amazon/aws/
---

# aws-vpc

Amazon Virtual Private Cloud. 
Build and launch resources in an isolated section of the AWS system.
You have complete control over the VPC details.

Subnet size range allowed in AWS VPC. 
```
*/16 (65,536) 
*/28 (256)
```

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