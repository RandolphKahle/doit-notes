---
date: 2020-10-02T13:37
tags:
  - amazon/aws/compute/ec2/
---


# EC2 Placement Group

A placement group provides control over the *physical* placement of virtual machines within availability zones.

The value of using a *placement group* is based on the relative performance, reliabilty, etc. of designating the proximity of various elements of compute (CPU, RAM, network, etc.)(e.g. a *rack*).

Restrictions: Name of placement gropu must be unique within an AWS account for a region. Dedicated Hosts are not supported.

## Cluster Placement Group


Packs instances close together inside a *single availability zone*.

![Cluster](./static/placement-group-cluster.png){.ui .center  .small .float .image}


Benefit: Low latency performance needed for tightly-coupled multinode compute deployment (e.g. HPC). 
Placed in the same high-biscetion bandwidth segment of the network.


## Partition Placement Group

Spreads instances across logical partitions *within a region* such that groups of instances are on separate hardware (such as separate racks).

![Cluster](./static/placement-group-partition.png){.ui .center  .medium .float .image}


Benefit: Reduces failure of entire compute deployment. Also, *placement information is shared with placement aware software* such as HDFS, HBase, and Cassandra.

Restriction: A *maximum of seven partitions per availability zone*.

Use case: HDFS, Cassandra, HBase.




## Spread Placement Group

Spreads instances across as much distinct hardware as possible *within a region*.

![Cluster](./static/placement-group-spread.png){.ui .center  .medium .float .image}


Use when there are a small number of instances that much be as isolated as possible.

Benefit: Reduce correlated failures.

Restriction: Maximum of seven running instances per availabilty zone per group.



### aws-compute-ec2-placement-group

