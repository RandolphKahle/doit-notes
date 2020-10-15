---
date: 2020-10-15T09:17
tags:
  - amazon/aws/security
---
# Parameter Store

Parameter Store is a component of [[[aws-ssm]]].

Serverless, scalable service:
* Save secrets:
  * Passwords
  * Database connection strings
  * License codes
  * API keys
* Values can be stored encrypted (KMS) or plaintext
* Separate data from source control
* Store in hierarchies and *fetch by path*
* Integrated with CloudFormation


Example path request:
```
/prod/db/mysql/db-string
```

CloudFormation integration example:
```
Parameters:
  LatestAmiId:
    Type: 'AWS::SSM::Parameter::Value<AWS::EC2::Image::Id>'
    Default: '/aws/service/ami-amazon-linux-latest/amxn2-ami-hvm-x86_64-gp2'
    
Resources:
  Instance:
    Type: 'AWS::EC2::Instance'
    Properties:
      ImageId: !Ref LatestAmiId
```
### aws-system-manager-parameter-store
