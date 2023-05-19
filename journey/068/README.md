
# Account Management, Billing & Support Section Part 3 (Udemy | Stephane Mareek)

## Cloud Research

### Compute Pricing – Lambda & ECS
- Lambda:
> • Pay per call

> • Pay per duration

- ECS:
> • EC2 Launch Type Model: No additional fees, you pay for AWS resources stored and created in your application

- Fargate: 
> • Fargate Launch Type Model: Pay for vCPU and memory resources allocated to your applications in your containers

### Storage Pricing – S3
- Storage class: S3 Standard, S3 Infrequent Access, S3 One-Zone IA, S3 
Intelligent Tiering, S3 Glacier and S3 Glacier Deep Archive
- Number and size of objects: Price can be tiered (based on volume)
- Number and type of requests
- Data transfer OUT of the S3 region
- S3 Transfer Acceleration
- Lifecycle transitions
- Similar service: EFS (pay per use, has infrequent access & lifecycle rules)

### Storage Pricing - EBS
- Volume type (based on performance)
- Storage volume in GB per month provisionned
- IOPS:
> • General Purpose SSD: Included

> • Provisioned IOPS SSD: Provisionned amount in IOPS

> • Magnetic: Number of requests

- Snapshots:
> • Added data cost per GB per month

- Data transfer:
> • Outbound data transfer are tiered for volume discounts

> • Inbound is free

### Database Pricing - RDS
- Per hour billing
- Database characteristics: 
> • Engine

> • Size

> • Memory class

- Purchase type:
> • On-demand

> • Reserved instances (1 or 3 years) with required up-front

- Backup Storage: There is no additional charge for backup storage up to 
100% of your total database storage for a region.

### Database Pricing - RDS
- Additional storage (per GB per month)
- Number of input and output requests per month
- Deployment type (storage and I/O are variable): 
> • Single AZ 

> • Multiple AZs

- Data transfer:

> • Outbound data transfer are tiered for volume discounts

> • Inbound is free

### Content Delivery – CloudFront
- Pricing is different across different geographic regions
- Aggregated for each edge location, then applied to your bill
- Data Transfer Out (volume discount)
- Number of HTTP/HTTPS requests

## Next Steps

- Account Management, Billing & Support Section Part 4