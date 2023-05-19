# Vpc Section Part 1 (Udemy | Stephane Mareek)

## Introduction

- VPC is something you should know in depth for the AWS Certified Solutions
  Architect Associate & AWS Certified SysOps Administrator

- At the AWS Certified Cloud Practitioner Level, you should know about:
  > • VPC, Subnets, Internet Gateways & NAT Gateways

> • Security Groups, Network ACL (NACL), VPC Flow Logs

> • VPC Peering, VPC Endpoints

> • Site to Site VPN & Direct Connect

> • Transit Gateway

## Cloud Research

### VPC & Subnets Primer

- VPC -Virtual Private Cloud: private network to deploy your resources
  (regional resource)
- Subnets allow you to partition your network inside your VPC
  (Availability Zone resource)
- A public subnet is a subnet that is
  accessible from the internet
- A private subnet is a subnet that is not
  accessible from the internet
- To define access to the internet and
  between subnets, we use Route Tables.

### Network ACL & Security Groups

- NACL (Network ACL)
> • A firewall which controls traffic from and to subnet

> • Can have ALLOW and DENY rules

> • Are attached at the Subnet level

> • Rules only include IP addresses

- Security Groups

> • A firewall that controls traffic to and from an ENI / an EC2 Instance

> • Can have only ALLOW rules

> • Rules include IP addresses and other security groups

### VPC Flow Logs

- Capture information about IP traffic going into your interfaces:
> • VPC Flow Logs

> • Subnet Flow Logs

> • Elastic Network Interface Flow Logs

- Helps to monitor & troubleshoot connectivity issues. Example:

> • Subnets to internet

> • Subnets to subnets

> • Internet to subnets

- Captures network information from AWS managed interfaces too: Elastic
  Load Balancers, ElastiCache, RDS, Aurora, etc…
- VPC Flow logs data can go to S3 / CloudWatch Logs

## Next Steps

- VPC Part 2
