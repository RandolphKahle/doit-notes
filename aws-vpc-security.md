---
date: 2020-10-14T09:35
tags:
  - amazon/aws/vpc/
  - network/security/
---
# VPC Security

Topics about VPC network security.

## General Techniques

* NACL to deny traffic from designated range of IP addresses
* Host based firewall, e.g. iptables
* Security Group
* Application Load Balancer challenges
  * ALB Security group -> EC2 Security Group
  * NACL in front of ALB
  * X-Forward-From HTTP header ?
* Network Load Balancer does not terminate client connection. (Layer 4)
  * NACL is only IP address defense.
* WAF Web Application Firewall (Layer 7)
  * Allow or Block based on conditions
  * XSS
  * SQL Injection
  * IP Blocking and Filtering
  * Geomatch for large block IP blocking
* CloudFront  
  * WAF attached.
  * Subsequent NACL is ineffective
  




### aws-vpc-security