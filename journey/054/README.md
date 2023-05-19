# Cloud Integration Section (Udemy | Stephane Mareek)

## Introduction

- When we start deploying multiple applications, they will inevitably need
  to communicate with one another
- Synchronous between applications can be problematic if there are
  sudden spikes of traffic
- What if you need to suddenly encode 1000 videos but usually it’s 10?
- In that case, it’s better to decouple your applications:
  > • using SQS: queue model
  > <br>• using SNS: pub/sub model
  > <br>• using Kinesis: real-time data streaming model
- These services can scale independently from our application!

## Cloud Research

### Amazon SQS – Standard Queue

- Oldest AWS offering (over 10 years old)
- Fully managed service (~serverless), use to decouple applications
- Scales from 1 message per second to 10,000s per second
- Default retention of messages: 4 days, maximum of 14 days
- No limit to how many messages can be in the queue
- Messages are deleted after they’re read by consumers
- Low latency (<10 ms on publish and receive)
- Consumers share the work to read messages & scale horizontally

### Amazon Kinesis

- For the exam: Kinesis = real-time big data streaming
- Managed service to collect, process, and analyze real-time streaming
  data at any scale
- Too detailed for the Cloud Practitioner exam but good to know:
  > • Kinesis Data Streams: low latency streaming to ingest data at scale from
  > hundreds of thousands of sources
  > <br>• Kinesis Data Firehose: load streams into S3, Redshift, ElasticSearch, etc…
  > <br>• Kinesis Data Analytics: perform real-time analytics on streams using SQL
  > <br>• Kinesis Video Streams: monitor real-time video streams for analytics or ML

### Amazon SNS

- The “event publishers” only sends message to one SNS topic
- As many “event subscribers” as we want to listen to the SNS topic notifications
- Each subscriber to the topic will get all the messages
- Up to 12,500,000 subscriptions per topic, 100,000 topics limit

### Amazon MQ

- SQS, SNS are “cloud-native” services: proprietary protocols from AWS
- Traditional applications running from on-premises may use open protocols such as: MQTT, AMQP, STOMP, Openwire, WSS
- When migrating to the cloud, instead of re-engineering the application to use SQS and SNS, we can use Amazon MQ
- Amazon MQ is a managed message broker service for
- Amazon MQ doesn’t “scale” as much as SQS / SNS
- Amazon MQ runs on servers, can run in Multi-AZ with failover
- Amazon MQ has both queue feature (~SQS) and topic features (~SNS)

## Next Steps

- Cloud Monitoring Section
