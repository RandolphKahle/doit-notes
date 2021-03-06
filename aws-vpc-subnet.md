---
date: 2020-10-05T07:10
tags:
  - amazon/aws/vpc/
---

# VPC subnet

[VPC](aws-vpc) subnets are a partioned subset CIDR block of
IP address from the containing VPC CIDR block.


For example, if the VPC has the CIDR block
```
10.0.0.0/16
```
Then the network addresses cannot overlap with a subnet.
Potential subnet CIDR blocks are then:
```
10.0.1.0/24
10.0.2.0/24
```

### Network Reserved Addresses
Amazon reserves five addresses from each subnet:
```
*.0 Network address
*.1 Outbound routing address
*.2 DNS
*.3 "Reserved for future use"
*.255 Broadcast (broadcast is *not* supported)
```


Subnet size range allowed in AWS VPC. 
```
*/16 (65536 - 65531 usable) 
*/28 (256 - 251 usable)
```



## EC2

[[aws-compute-ec2]] instances must be bound to a VPC subnet
and cannot be bound to the [[aws-vpc]] CIDR block.



aws-vpc-subnet