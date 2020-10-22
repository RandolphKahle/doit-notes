---
date: 2020-10-08T22:11
tags:
  - amazon/aws/vpc/connection/
---

# VPC Peering

Allow you to connect one VPC with another using private IP 
addresses.

* Instance behave as if they are on the same VPC
* Peer with other VPC in the same account
* Peer with other VPC in another account
* Peer with another VPC in a different [[aws-region]].
* *Not* transitive. Peers can only forward to their directly connected VPCs.

### aws-vpc-connection-peering