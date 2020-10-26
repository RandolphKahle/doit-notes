---
date: 2020-10-04T09:05
tags:
  - amazon/aws/dns/
---

# aws-dns-routing

Types of Route53 routing:
* Simple 
* Failover
* Geolocation
* Geoproximity 
* Latency-based
* Multi-value answer
* Weighted


## Simple Routing Policy

One entry with one IP address.

## Failover Routing Policy

One entry with a primary and backup IP addresses.

A health-check is used to confirm if the service at the primary address is healthy and active. If not, then the alternate IP address is returned. 
(What about health check with backup?)

Used for an active / passive setup. For example,
us-east-1 might be the active region and ap-southeast-2 might be the backup.

## Geolocation Routing Policy

Select destination for traffic based on location of the user—based on continent or country.

For example, a European customer will be routed to the european region.

## Geoproximity Routing

Determines the distance of a user from different regions, such
as US-EAST-1 or US-WEST-1.

Route53 routes based on location of user and resources.
Can apply a bias which will compress or expand a geographic region.

Uses *Route 53 Traffic Flow*.

## Latency Based Routing Policy

Determines the latency between the user and different resources.
Sends user to destination with lowest latency.

?how does it know?



## Multi-Value Answer Routing

Similar to Simple Routing except you can associate a group of destinations and all are sent back. 
The client will pick one.


## Weighted Routing Policy

You can distribute your traffic with a weighting bias. For example, 10% to one IP address and 90% to another IP address.




