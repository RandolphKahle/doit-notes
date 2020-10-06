---
date: 2020-10-06T10:15
tags:
  - amazon/aws/storage/gateway/
---

# aws-transit-gateway

Designed to simplify an involved network design.
Simplifies the case where an on-premise data center has multiple VPN connections to AWS with multiple entry points, etc.

With transit gateway a single gateway is used as an entry point and then acts a the hub in a hub-and-spoke architecture.
Connections are delegated out to the appropriate locations within AWS.

Regional. But can be used cross-region.

Supports [[network-protocol-multicast]].


