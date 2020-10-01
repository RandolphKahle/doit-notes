---
date: 2020-10-01T08:42
tags:
  - amazon/aws/compute/ec2/
---

# aws-compute-ec2-instance-store

An **Instance Store** or **Ephemeral Storage** is a block storage device (exclusively SSD?) that is hosted on the physical server where the virtual machine runs. 

These only persist through a reboot and not through a stop on the instance. Good for temporary high-performance storage or in a [[high-availability-architecture]] design.