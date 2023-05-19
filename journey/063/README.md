
# Security & Compliance Section Part 3 (Udemy | Stephane Mareek)

## Cloud Research

### CloudHSM
- KMS => AWS manages the software 
for encryption
- CloudHSM => AWS provisions 
encryption hardware
- Dedicated Hardware (HSM = 
Hardware Security Module)
- You manage your own encryption 
keys entirely (not AWS)
- HSM device is tamper resistant, FIPS 
140-2 Level 3 compliance

### AWS Certificate Manager (ACM) 
- Let’s you easily provision, manage, and deploy 
SSL/TLS Certificates
- Used to provide in-flight encryption for websites (HTTPS)
- Supports both public and private TLS 
certificates
- Free of charge for public TLS certificates
- Automatic TLS certificate renewal
- Integrations with (load TLS certificates on)
> • Elastic Load Balancers

> • CloudFront Distributions

> • APIs on API Gateway

### AWS Secrets Manager
- Newer service, meant for storing secrets
- Capability to force rotation of secrets every X days
- Automate generation of secrets on rotation (uses Lambda)
- Integration with Amazon RDS (MySQL, PostgreSQL, Aurora)
- Secrets are encrypted using KMS
- Mostly meant for RDS integration

### Amazon GuardDuty
- Intelligent Threat discovery to Protect AWS Account 
- Uses Machine Learning algorithms, anomaly detection, 3rd party data
- One click to enable (30 days trial), no need to install software
- Input data includes:
> - CloudTrail Events Logs – unusual API calls, unauthorized deployments

> > • CloudTrail Management Events – create VPC subnet, create trail, …

> > • CloudTrail S3 Data Events – get object, list objects, delete object, …
> - VPC Flow Logs – unusual internal traffic, unusual IP address

> - DNS Logs – compromised EC2 instances sending encoded data within DNS queries

> - Kubernetes Audit Logs – suspicious activities and potential EKS cluster compromises

- Can setup CloudWatch Event rules to be notified in case of findings
- CloudWatch Events rules can target AWS Lambda or SNS
- Can protect against CryptoCurrency attacks (has a dedicated “finding” for it)


### AWS Config
- Helps with auditing and recording compliance of your AWS resources
- Helps record configurations and changes over time
- Possibility of storing the configuration data into S3 (analyzed by Athena)
- Questions that can be solved by AWS Config: 
> • Is there unrestricted SSH access to my security groups?

> • Do my buckets have any public access?

> • How has my ALB configuration changed over time?

- You can receive alerts (SNS notifications) for any changes
- AWS Config is a per-region service
- Can be aggregated across regions and accounts

### AWS Macie
- Amazon Macie is a fully managed data security and data privacy service 
that uses machine learning and pattern matching to discover and protect your sensitive data in AWS.
- Macie helps identify and alert you to sensitive data, such as personally identifiable information (PII)

### AWS Security Hub
- Central security tool to manage security across several AWS accounts and 
automate security checks
- Integrated dashboards showing current security and compliance status to quickly 
take actions
- Automatically aggregates alerts in predefined or personal findings formats from 
various AWS services & AWS partner tools: 
> • GuardDuty

> • Inspector

> • Macie

> • IAM Access Analyzer

> • AWS Systems Manager

> • AWS Firewall Manager

> • AWS Partner Network Solutions

- Must first enable the AWS Config Service

### Amazon Detective
- GuardDuty, Macie, and Security Hub are used to identify potential 
security issues, or findings
- Sometimes security findings require deeper analysis to isolate the root 
cause and take action – it’s a complex process
- Amazon Detective analyzes, investigates, and quickly identifies the root 
cause of security issues or suspicious activities (using ML and graphs)
- Automatically collects and processes events from VPC Flow Logs, 
CloudTrail, GuardDuty and create a unified view
- Produces visualizations with details and context to get to the root cause

### AWS Abuse
- Report suspected AWS resources used for abusive or illegal purposes
- Abusive & prohibited behaviors are: 
> • Spam – receving undesired emails from AWS-owned IP address, websites & forums spammed by AWS resources

> • Port scanning – sending packets to your ports to discover the unsecured ones

> • DoS or DDoS attacks – AWS-owned IP addresses attempting to overwhlem or crash your servers/softwares

> • Intrusion attempts – logging in on your resources

> • Hosting objectionable or copyrighted content – distributing illegal or copyrighted content without consent

> • Distributing malware – AWS resources distributing softwares to harm computers or machines

- Contact the AWS Abuse team: AWS abuse form, or abuse@amazonaws.com

## Next Steps

- Machine Learning Section Part 1