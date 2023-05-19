
# Security & Compliance Section Part 1 (Udemy | Stephane Mareek)

## Cloud Research

### AWS Shared Responsibility Model
- AWS responsibility - Security of the Cloud
>• Protecting infrastructure (hardware, software, facilities, and networking) that runs  all the AWS services

> • Managed services like S3, DynamoDB, RDS, etc.

- Customer responsibility - Security in the Cloud
> • For EC2 instance, customer is responsible for management of the guest OS (including security patches and updates), firewall & network configuration, IAM 

> • Encrypting application data 

- Shared controls:
> • Patch Management, Configuration Management, Awareness & Training

### Example, for RDS
- AWS responsibility:
> • Manage the underlying EC2 instance, disable SSH access

> • Automated DB patching

> • Automated OS patching

> • Audit the underlying instance and disks & guarantee it functions

- Your responsibility:
> • Check the ports / IP / security group inbound rules in DB’s SG

> • In-database user creation and permissions

> • Creating a database with or without public access

> • Ensure parameter groups or DB is configured to only allow SSL connections

> • Database encryption setting


### DDOS Protection on AWS
- AWS Shield Standard: protects against DDOS attack for your website 
and applications, for all customers at no additional costs
- AWS Shield Advanced: 24/7 premium DDoS protection
- AWS WAF: Filter specific requests based on rules
- CloudFront and Route 53: 
> • Availability protection using global edge network
> • Combined with AWS Shield, provides attack mitigation at the edge

- Be ready to scale – leverage AWS Auto Scaling

### AWS Shield
- AWS Shield Standard:
> • Free service that is activated for every AWS customer

> • Provides protection from attacks such as SYN/UDP Floods, Reflection attacks and other layer 3/layer 4 attacks

- AWS Shield Advanced: 
> • Optional DDoS mitigation service ($3,000 per month per organization) 

> • Protect against more sophisticated attack on Amazon EC2, Elastic Load Balancing (ELB), Amazon CloudFront, AWS Global Accelerator, and Route 53

> • 24/7 access to AWS DDoS response team (DRP)

> • Protect against higher fees during usage spikes due to DDoS

### AWS WAF – Web Application Firewall
- Protects your web applications from common web exploits (Layer 7)

- Layer 7 is HTTP (vs Layer 4 is TCP)

- Deploy on Application Load Balancer, API Gateway, CloudFront

- Define Web ACL (Web Access Control List):
> • Rules can include IP addresses, HTTP headers, HTTP body, or URI strings

> • Protects from common attack - SQL injection and Cross-Site Scripting (XSS)

> • Size constraints, geo-match (block countries)

> • Rate-based rules (to count occurrences of events) – for DDoS protection


## Next Steps

- Security & Compliance Section Part 2
