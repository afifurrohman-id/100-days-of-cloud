# Load Balancing (Udemy | Stephane Mareek)

## Introduction

Load balancers are servers that forward internet traffic to multiple servers (EC2 Instances) downstream.

## Cloud Research

### Why use a load balancer?

- Spread load across multiple downstream instances
- Expose a single point of access (DNS) to your application
- Seamlessly handle failures of downstream instances
- Do regular health checks to your instances
- Provide SSL termination (HTTPS) for your websites
- High availability across zones

### Why use an Elastic Load Balancer?

- An ELB (Elastic Load Balancer) is a managed load balancer
  > AWS guarantees that it will be working <br> AWS takes care of upgrades, maintenance, high availability <br> AWS provides only a few configuration knobs <br>
- It costs less to setup your own load balancer but it will be a lot more
  effort on your end (maintenance, integrations)
- 4 kinds of load balancers offered by AWS:
  > Application Load Balancer (HTTP / HTTPS only) – Layer 7 <br> Network Load Balancer (ultra-high performance, allows for TCP) – Layer 4 <br> Gateway Load Balancer – Layer 3 <br> Classic Load Balancer (retired in 2023) – Layer 4 & 7

## Next Steps

- Auto Scaling Group
