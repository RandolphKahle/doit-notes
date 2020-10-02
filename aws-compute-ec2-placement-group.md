---
date: 2020-10-02T13:37
tags:
  - amazon/aws/compute/ec2/
---

# aws-compute-ec2-placement-group

# EC2 Placement Group

A placement group provides control over the *physical* placement of virtual machines within an availability zone.

The value is predicated on localized placement relative to network instance and shared infrastructure (e.g. a *rack*).

## Cluster Placement Group

Supports the co-location of a set of virtual machines in the same rack, on the same physical network. This provides the highest network throughput and lowest latency.

## Spread Placement Group

Supports the non-co-location of a set of virtual machines on different racks. This provides the highest degree of conincident failure of virtual machines within the same availability zone.

## Partition Placement Group

Supports the co-location of virtual machines in a partition and the spreading of multiple partitions across racks.

