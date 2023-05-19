# AWS Snow Family (Udemy | Stephane Mareek)

## Introduction

The AWS Snow Family is a collection of physical devices that help migrate large amounts of data into and out of the cloud without depending on networks. This helps you apply the wide variety of AWS services for analytics, file systems, and archives to your data.

## Cloud Research

### Snowball Edge (for data transfers)

- Physical data transport solution: move TBs or PBs of data in or out
  of AWS
- Alternative to moving data over the network (and paying network
  fees)
- Pay per data transfer job
- Provide block storage and Amazon S3 - compatible object storage
- Snowball Edge Storage Optimized
  > • 80 TB of HDD capacity for block volume and S3 compatible object
  > storage
- Snowball Edge Compute Optimized
  > • 42 TB of HDD capacity for block volume and S3 compatible object
  > storage
- Use cases: large data cloud migrations, DC decommission, disaster
  recovery

### AWS Snowcone

- Small, portable computing, anywhere, rugged &
  secure, withstands harsh environments
- Light (4.5 pounds, 2.1 kg)
- Device used for edge computing, storage, and data
  transfer
- 8 TBs of usable storage
- Use Snowcone where Snowball does not fit
  (space
  -constrained environment)
- Must provide your own battery / cables
- Can be sent back to AWS offline, or connect it to
  internet and use AWS DataSync to send data

### AWS Snowmobile

- Transfer exabytes of data (1 EB = 1,000 PB = 1,000,000 TBs)
- Each Snowmobile has 100 PB of capacity (use multiple in parallel)
- High security: temperature controlled, GPS, 24/7 video surveillance
- Better than Snowball if you transfer more than 10 PB

### Snow Family – Usage Process

1. Request Snowball devices from the AWS console for delivery
2. Install the snowball client / AWS OpsHub on your servers
3. Connect the snowball to your servers and copy files using the client
4. Ship back the device when you’re done (goes to the right AWS
   facility)
5. Data will be loaded into an S3 bucket
6. Snowball is completely wiped

### What is Edge Computing?

- Process data while it’s being created on an edge location
  > • A truck on the road, a ship on the sea, a mining station underground...
- These locations may have
  > • Limited / no internet access
  > <br>• Limited / no easy access to computing power
- We setup a Snowball Edge / Snowcone device to do edge computing
- Use cases of Edge Computing:
  > • Preprocess data
  > <br>• Machine learning at the edge
  > <br>• Transcoding media streams
- Eventually (if need be) we can ship back the device to AWS (for transferring data for example)

### Snow Family – Edge Computing

- Snowcone (smaller)
  > • 2 CPUs, 4 GB of memory, wired or wireless access
  > <br>• USB-C power using a cord or the optional battery
- Snowball Edge – Compute Optimized
  > • 52 vCPUs, 208 GiB of RAM
  > <br>• Optional GPU (useful for video processing or machine learning)
  > <br>• 42 TB usable storage
- Snowball Edge – Storage Optimized
  > • Up to 40 vCPUs, 80 GiB of RAM
  > <br>• Object storage clustering available
- All: Can run EC2 Instances & AWS Lambda functions (using AWS IoT Greengrass)
- Long-term deployment options: 1 and 3 years discounted pricing

## Next Steps

- Meet 3 (Setting Adapter, Ip Address Vm, Connect vm to internet & Host OS)
