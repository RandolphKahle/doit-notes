---
date: 2020-10-09T14:19
tags:
  - amazon/aws/vpc/
---

# aws-vpc-global-accelerator
# Global Accelerator


A Global Accelerator offers a connection into the Amazon
backbone network located as close as possible to end users. 

The user-facing point is an Amazon Edge Location. The Amazon facing location is a *network zone* (not an availability zone). 


![Global Accelerator](./static/aga_ip_preservation_alb.png)

![Non accelerated path](./static/non-accelerator.png)

![Accelerated Path](./static/accelerator.png)
