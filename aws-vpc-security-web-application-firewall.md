---
date: 2020-10-14T09:58
tags:
  - amazon/aws/vpc/security/
  - network/security/
---

# Web Application Firewall (WAF)

Web application that monitors HTTP and HTTPS requests to
* CloudFront
* Application Load Balancer (ALB)
* API Gateway

Is tightly integrated with [[aws-vpc-security-firewall-manager]]

Control access to content via *filtering rules*
* IP Address of source
* Source country
* Request size
* Header values
* Regex pattern matching (e.g. for User Agent Header)
* Query string parameters
* SQL query injection attacks
* XSS attacks (Cross-site scripting)



Returns an HTTP 403 return code

* Allow all, except specified
* Block all, except specified
* Count all as specified


### aws-vpc-security-web-application-firewall