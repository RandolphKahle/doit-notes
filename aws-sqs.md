---
date: 2020-10-14T17:20
tags:
  - amazon/aws/
---

# Simple Queue Service

Original AWS service.

* Distributed message queue system
* Pull based system
* Message size
  * 256K in-message
  * 2GB in S3
* Type
  * Standard (no ordering, deliver at least once, no order)
    * Extremely high through-put
  * FIFO (guaranteed order, deliver once)
    * 300 TPS

### Notes
#### Visibility timeout 
The time a message is hidden during client processing. If the client fails to process within this window then the message reappears in the queue.   
Maximum 12 hours.

Use *long-polling* to reduce chatter and cost.

### aws-sqs