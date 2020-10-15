---
date: 2020-10-15T05:59
tags:
  - amazon/aws/
---
# Cognito

Cognito is a web identity federation service.

Coordinates authentication using services such as Facebook, Google, etc.

Essentially Cognito maps between Google authentication tokens and an IAM role within AWS.

* Access for guest
* Identity broker between an application and Web ID providers
* Synchronizes user data for multiple devices

## User Pool

A user directory managing sign-up and sign-in functionality for web and mobile applications. 
Users sign-in directly to the User Pool or using Facebook, Amazon, or Google.
Successful authentication generates a JWT.

## Identity Pool

### aws-cognito