# EFS – Elastic File System (Udemy | Stephane Mareek)

## Introduction

Amazon Elastic File System (Amazon EFS) is a simple, serverless, set-and-forget, elastic file system. There is no minimum fee or setup charge. You pay only for the storage you use, for read and write access to data stored in Infrequent Access storage classes, and for any provisioned throughput. The journey will be like this:

- EFS – Elastic File System Intro
- EFS Infrequent Access (EFS-IA)

## Cloud Research

### EFS – Elastic File System

- Managed NFS (network file system) that can be mounted on 100s of EC2
- EFS works with Linux EC2 instances in multi-AZ
- Highly available, scalable, expensive (3x gp2), pay per use, no capacity planning

### EFS Infrequent Access (EFS-IA)

- Storage class that is cost-optimized for files not
  accessed every day
- Up to 92% lower cost compared to EFS Standard
- EFS will automatically move your files to EFS-IA
  based on the last time they were accessed
- Enable EFS-IA with a Lifecycle Policy
- Example: move files that are not accessed for 60
  days to EFS-IA
- Transparent to the applications accessing EFS

## Next Steps

- Amazon FSx

