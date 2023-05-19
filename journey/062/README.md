
# Security & Compliance Section Part 2 (Udemy | Stephane Mareek)

## Cloud Research

### Penetration Testing on AWS Cloud
- AWS customers are welcome to carry out security assessments or 
penetration tests against their AWS infrastructure without prior approval for 8 services: 

> • Amazon EC2 instances, NAT Gateways, and Elastic Load Balancers

> • Amazon RDS

> • Amazon CloudFront

> • Amazon Aurora

> • Amazon API Gateways

> • AWS Lambda and Lambda Edge functions

> • Amazon Lightsail resources

> • Amazon Elastic Beanstalk environments

- List can increase over time (you won’t be tested on that at the exam)

### Data at rest vs. Data in transit
- At rest: data stored or archived on a device
> • On a hard disk, on a RDS instance, in S3 Glacier Deep Archive, etc.
- In transit (in motion): data being moved from one location to another

> • Transfer from on-premises to AWS, EC2 to DynamoDB, etc.

> • Means data transferred on the network
- We want to encrypt data in both states to protect it!
- For this we leverage encryption keys

### AWS KMS (Key Management Service)
- Anytime you hear “encryption” for an AWS service, it’s most likely KMS
- KMS = AWS manages the encryption keys for us
- Encryption Opt-in:
> • EBS volumes: encrypt volumes

> • S3 buckets: Server-side encryption of objects

> • Redshift database: encryption of data

> • RDS database: encryption of data

> • EFS drives: encryption of data

- Encryption Automatically enabled: 
> • CloudTrail Logs

> • S3 Glacier

> • Storage Gateway


## Next Steps

- Security & Compliance Section Part 3

