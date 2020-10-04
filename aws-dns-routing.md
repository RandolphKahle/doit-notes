---
date: 2020-10-04T09:05
tags:
  - amazon/aws/dns/
---

# aws-dns-routing

Types of Route53 routing:
* Simple 
* Weighted
* Latency-based
* Failover
* Geolocation
* Geoproximity 
* Multi-value answer

## Simple Routing Policy

One entry with multiple IP addresses. Route53 returns an IP address selected at random from the set for each query.

## Weighted Routing Policy

You can distribute your traffic with a weighting bias. For example, 10% to one IP address and 90% to another IP address.

## Latency Based Routing Policy

Determines which region exhibits the lowest latency for a user.

