---
date: 2020-10-14T09:58
tags:
  - amazon/aws/vpc/security/
  - network/security/
---


# Firewall Manager

Security application that centralizes control over firewall
rules across an [[aws-organization]].

Tightly integrated with [[aws-vpc-security-web-application-firewall]].

* WAF rules managed on
  * ALB
  * API Gateway
  * CloudFront distributions
* Advanced [[aws-vpc-security-shield]] protections:
  * ALB
  * ELB Classic
  * EIP
  * CloudFront distributions
* Enable security groups for [[aws-compute-ec2]] and [[aws-vpc-elastic-network-interface]].




### aws-vpc-security-firewall-manager