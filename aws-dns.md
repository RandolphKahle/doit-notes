---
date: 2020-10-03T16:44
tags:
  - amazon/aws/
---

# aws-dns

Amazon Domain Name Service - Route 53.

Start of Authority (SOA) -
* Name of the server that supplies information for the zone
* Administrator
* Version of the file
* Default TTL for information in the file

Name Server record (NS) -

These are used by the top-level domain servers to hold the address of the content DNS server which contains the authoratative DNS records.

Address record (A)

The fundamental type of record. It contains a direct mapping of a name to an IP address.

TTL

Time to live for most records is 48 hours (172800 seconds).

Canonical Name (CNAME)



