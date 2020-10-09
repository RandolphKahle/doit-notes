---
date: 2020-10-09T14:19
tags:
  - amazon/aws/vpc/
---

# aws-vpc-global-accelerator
# Global Accelerator


A Global Accelerator provides a mechanism to avoid sending network traffic from a user to resources in AWS across a portion of the public internet.

Amazon has AWS *edge locations* in many parts of the world. One side of an edge location connects to the public internet and the other to the Amazon backbone network. Instead of having traffic route through many ISPs on the way to Amazon, as illustrated:

![Non accelerated path](./static/non-accelerator.png){.ui .centered .image}  

The Global Accelerator provides a more direct path, as illustrated:

![Accelerated Path](./static/accelerator.png){.ui .centered .image}    
On the Amazon side, the connection terminates at one of two IP addresses. Each in their own *network zone*. Two addresses are provided for HA redundancy.

On the client-facing side, there are listener processes that support TCP and UDP and can be configured for one or more IP ports. 
The listeners are ?associated? with an (or more?) endpoint groups.




![Global Accelerator](./static/aga-ip-preservation-alb.png){.ui .centered .image}      

