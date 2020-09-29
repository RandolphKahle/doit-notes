---
date: 2020-09-29T14:29
tags:
  - amazon/aws/storage/s3/
---

# aws-s3-worm

**Update this section from the aCloud.guru class before exam**

S3 Governance Mode  
User needs special permission to alter the object

S3 Compliance Mode  
No one can change or delete the object until the end of the
retention period. After that time, then someone can alter or delete.


S3 Legal Hold  
Does not have a retension period, however, a user needs the s3:PutObjectLegalHold permission.

Glacier  
Prevent deletion. Once set, cannot be removed (?)


S3 Object Lock can be configured in one of two Modes. When deployed in Governance Mode, AWS accounts with specific IAM permissions are able to remove WORM protection from an object. If you require stronger immutability in order to comply with regulations, you can use Compliance Mode. In Compliance Mode, WORM protection cannot be removed by any user, including the root account.

Alternatively, you can make an object immutable by applying a Legal Hold to that object. A Legal Hold places indefinite S3 Object Lock protection on an object, which will remain until it is explicitly removed. In order to place and remove Legal Holds, your AWS account must have write permission for the PutObjectLegalHold action. Legal Hold can be applied to any object in an S3 Object Lock enabled bucket, whether or not that object is currently WORM-protected by a retention period.