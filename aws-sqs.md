---
date: 2020-10-14T17:20
tags:
  - amazon/aws/
---

# Simple Queue Service

Original AWS service.

* Distributed message queue system
* Retention up to 14 days (default is 4 days)
* Pull based system
* Message size
  * 256K in-message
  * 2GB in S3
    
## Type

### Standard
  * No order
  * Deliver at least once
  * Extremely high throughput
### FIFO
  * Guaranteed order
  * Deliver once
  * 300 TPS

## Notes
#### Visibility timeout 
The time a message is hidden during client processing. If the client fails to process within this window then the message reappears in the queue.   
Maximum 12 hours.

Use *long-polling* to reduce chatter and cost.

### aws-sqs