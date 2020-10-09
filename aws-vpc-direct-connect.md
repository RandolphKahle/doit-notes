---
date: 2020-10-09T07:48
tags:
  - amazon/aws/vpc/
---

# aws-vpc-direct-connect
# Direct Connect
Establish a *dedicated* network connection between external location and AWS.
Because it is a dedicated 'wire' it is inherently **more secure** than a virtual circuit across the public internet.

Connect to a Direct Connect location (DX). 
We are talking about cage to cage connection with a physical line.

From the aCloud.guru course it appears that there is a "public" and a "private" virtual circuit. Public going to services such as S3 and private going to, e.g., our VPCs.

* Reduce network costs
* Increase consistency
* Increase bandwidth

AWS Direct Connect offers:
* Public Virtual Interface
* Private Virtual Interface
* Transit Virtual Interface



## Sets to set up a Direct Connection
* Create a Public Virtual Interface (for ...)
* Create a Customer Gateway in the VPN configuration section of VPC
* Create a Virtual Private Gateway
* Attach the Virtual Private Gateway to the desired VPC
* Creata a new VPN connection
* Select:
  * Virtual Private Gateway
  * Customer Gateway
* Set up the VPN circuit on the customer hardware side of the connection.
