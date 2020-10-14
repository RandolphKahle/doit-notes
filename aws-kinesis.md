---
date: 2020-10-14T17:55
tags:
  - amazon/aws/
---

# Kinesis

System supporting streaming of small parcels of data. Think IoT type systems.

* On-line store purchases
* Stock pricess
* Game data
* Twitter
* Geospacial (e.g. Uber)
* IoT sensors

### Kinesis Streams

Separate streams. Stored in **shards**. Generally sent to EC2 instances.

24 hour? 7 Day rentention?

5 Transactions per second for reads

1,000 records per second writes

Capacity is based on the number of shards.
### Kinesis Firehose

**No persistence**. Must be processed on arrival. Lamda function is ideal. Process and deliver.

### Kinesis Analytics

Analyze data on the fly in either of the above services.


### aws-kinesis