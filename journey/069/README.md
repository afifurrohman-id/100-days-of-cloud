
# Account Management, Billing & Support Section Part 4 (Udemy | Stephane Mareek)

## Cloud Research

### Savings Plan
- Commit a certain $ amount per hour for 1 or 3 years 
- Easiest way to setup long-term commitments on AWS
- EC2 Savings Plan
> • Up to 72% discount compared to On-Demand

> • Commit to usage of individual instance families in a region (e.g. C5 or M5)

> • Regardless of AZ, size (m5.xl to m5.4xl), OS (Linux/Windows) or tenancy

> • All upfront, partial upfront, no upfront

- Compute Savings Plan
> • Up to 66% discount compared to On-Demand

> • Regardless of Family, Region, size, OS, tenancy, compute options

> • Compute Options: EC2, Fargate, Lambda

- Machine Learning Savings Plan: SageMaker… 
- Setup from the AWS Cost Explorer console
- Estimate pricing at https://aws.amazon.com/savingsplans/pricing/

### AWS Compute Optimizer
- Reduce costs and improve performance by recommending optimal AWS resources for your 
workloads
- Helps you choose optimal configurations and right- size your workloads (over/under provisioned)
- Uses Machine Learning to analyze your resources’ 
configurations and their utilization CloudWatch 
metrics
- Supported resources
> • EC2 instances

> • EC2 Auto Scaling Groups

> • EBS volumes

> • Lambda functions

- Lower your costs by up to 25%

- Recommendations can be exported to S3

### Billing and Costing Tools
- Estimating costs in the cloud:
> • Pricing Calculator

- Tracking costs in the cloud:
> • Billing Dashboard

> • Cost Allocation Tags

> • Cost and Usage Reports

> • Cost Explorer

- Monitoring against costs plans:
> • Billing Alarms

> • Budgets

### AWS Pricing Calculator
- Available at https://calculator.aws/
- Estimate the cost for your solution architecture

### Cost and Usage Reports
- Dive deeper into your AWS costs and usage
- The AWS Cost & Usage Report contains the most comprehensive set of AWS cost and usage data available, including additional metadata 
about AWS services, pricing, and reservations (e.g., Amazon EC2 Reserved Instances (RIs)).
- The AWS Cost & Usage Report lists AWS usage for each service 
category used by an account and its IAM users in hourly or daily line 
items, as well as any tags that you have activated for cost allocation 
purposes.
- Can be integrated with Athena, Redshift or QuickSight

### Cost Explorer
- Visualize, understand, and manage your AWS costs and usage over time
- Create custom reports that analyze cost and usage data. 
- Analyze your data at a high level: total costs and usage across all accounts 
- Or Monthly, hourly, resource level granularity
- Choose an optimal Savings Plan (to lower prices on your bill)
- Forecast usage up to 12 months based on previous usage

#### Billing Alarms in CloudWatch
- Billing data metric is stored 
in CloudWatch us-east-1 
- Billing data are for overall 
worldwide AWS costs
- It’s for actual cost, not for 
projected costs
- Intended a simple alarm 
(not as powerful as AWS 
Budgets)

### AWS Budgets
- Create budget and send alarms when costs exceeds the budget
- 3 types of budgets: Usage, Cost, Reservation
- For Reserved Instances (RI)
>• Track utilization

>• Supports EC2, ElastiCache, RDS, Redshift

- Up to 5 SNS notifications per budget
- Can filter by: Service, Linked Account, Tag, Purchase Option, Instance 
Type, Region, Availability Zone, API Operation, etc… 
- Same options as AWS Cost Explorer!
- 2 budgets are free, then $0.02/day/budget

### Trusted Advisor
- No need to install anything – high level 
AWS account assessment
- Analyze your AWS accounts and provides 
recommendation on 5 categories
- Cost optimization
- Performance
- Security
- Fault tolerance
- Service limits

## Next Steps

- Account Management, Billing & Support Section Part 5