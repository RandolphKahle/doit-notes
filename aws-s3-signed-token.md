---
date: 2020-09-29T17:41
tags:
  - amazon/aws/storage/s3/security/
---

# aws-s3-signed-token

A signed resource identifier that allows the holder to perform certain actions against the resource, e.g., GET.

Attach a policy to the cookie or URL
* URL experiation
* IP address range
* Trusted signers

## CDN

Create a distribution.

Signed URL or signed cookie.

Uses [[security-origin-access-identity]] Origin Access Identity (OAI) to associate (connect to/with (?) an S3 bucket).

### Signed URL

Gives authorization for a single resource.

### Cookie

Good for access to multiple files.

## S3

Signed URL.

Acts as an IAM user with their permissions. Has a limited life-time.

