
# VPC Part 2 (Udemy | Stephane Mareek)

## Cloud Research

### VPC Peering
- Connect two VPC, privately using 
AWS’ network
- Make them behave as if they were 
in the same network
- Must not have overlapping CIDR (IP 
address range)
- VPC Peering connection is not 
transitive (must be established for 
each VPC that need to 
communicate with one another)

### VPC Endpoints
- Endpoints allow you to connect to AWS 
Services using a private network instead 
of the public www network
- This gives you enhanced security and 
lower latency to access AWS services
- VPC Endpoint Gateway: S3 & DynamoDB
- VPC Endpoint Interface: the rest

### AWS PrivateLink (VPC Endpoint Services)
- Most secure & scalable way to expose a service to 1000s of VPCs
- Does not require VPC peering, internet gateway, NAT, route tables…
- Requires a network load balancer (Service VPC) and ENI (Customer VPC)


### Site to Site VPN & Direct Connect
- Site to Site VPN
> • Connect an on-premises VPN to AWS

> • The connection is automatically encrypted

> • Goes over the public internet

- Direct Connect (DX)
> • Establish a physical connection between  on-premises and AWS

> • The connection is private, secure and fast

> • Goes over a private network

> • Takes at least a month to establish

### AWS Client VPN
- Connect from your computer using OpenVPN to your private network 
in AWS and on-premises
- Allow you to connect to your EC2 instances over a private IP (just as if 
you were in the private VPC network)
- Goes over public Internet

### Transit Gateway
- For having transitive peering 
between thousands of VPC and 
on-premises, hub-and-spoke (star) 
connection
- One single Gateway to provide 
this functionality
- Works with Direct Connect 
Gateway, VPN connections

## Next Steps

- Security & Compliance Section Part 1
