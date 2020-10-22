---
date: 2020-10-01T08:42
tags:
  - amazon/aws/vpc/
---


# Network Interface

**ENI** is a virtual network interface card.

Use case: basic networking

* One primary *private* IPv4 address
* Multiple secondary *private* IPv4 addresses
* One elastic IPv4 address for each private IPv4 address
* One *public* IPv4 address
* Multiple IPv6 addresses
* One or more [[aws-compute-network-security-group]]s.
* One MAC address
* Source/Destination check flag ???
* Description


**ENA** is sub-set of **EN**, *enhanced networking*. 

Use case: high-performance networking.

This uses single-root-io-virtualization (SR-IOV) for enhanced network performance.

There is no additional charge for this level of networking, it is only limited by intance type support.

Two ways to activate EN:
* ENA - Enhanced network adapter (up to 100GBs)
* Intel 82599 virtualization (up to 10GBs)

**EFA** is *elastic fabric adapter*

Use case: High Performance Computing cluster configurations.

Does not use TCP/IP (what does it use?) for HPC builds.
Bypasses the OS and talks directly to the EFA.

From Amazon:
>With EFA, High Performance Computing (HPC) applications using the Message Passing Interface (MPI) and Machine Learning (ML) applications using NVIDIA Collective Communications Library (NCCL) can scale to thousands of CPUs or GPUs. 

### aws-vpc-interface
