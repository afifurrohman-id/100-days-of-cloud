# Auto Scaling Group Intro (Udemy | Stephane Mareek)

## Introduction

An Auto Scaling group contains a collection of EC2 instances that are treated as a logical grouping for the purposes of automatic scaling and management. An Auto Scaling group also lets you use Amazon EC2 Auto Scaling features such as health check replacements and scaling policies.

## Cloud Research

### Auto Scaling Group

- In real-life, the load on your websites and application can change
- In the cloud, you can create and get rid of servers very quickly
- The goal of an Auto Scaling Group (ASG) is to:
  > • Scale out (add EC2 instances) to match an increased load
  > <br>• Scale in (remove EC2 instances) to match a decreased load
  > <br>• Ensure we have a minimum and a maximum number of machines running
  > <br>• Automatically register new instances to a load balancer
  > <br>• Replace unhealthy instances
- Cost Savings: only run at an optimal capacity (principle of the cloud)

### Auto Scaling Groups – Scaling Strategies

- Manual Scaling: Update the size of an ASG manually
- Dynamic Scaling: Respond to changing demand

##### Simple / Step Scaling

> • When a CloudWatch alarm is triggered (example CPU > 70%), then add 2 units
> <br>• When a CloudWatch alarm is triggered (example CPU < 30%), then remove 1

##### Target Tracking Scaling

> • Example: I want the average ASG CPU to stay at around 40%

##### Scheduled Scaling

> • Anticipate a scaling based on known usage patterns
> <br>• Example: increase the min. capacity to 10 at 5 pm on Fridays

- Predictive Scaling
  > • Uses Machine Learning
  > to predict future traffic
  > ahead of time
  > <br>• Automatically
  > provisions the right
  > number of EC2
  > instances in advance
- Useful when your load
  has predictable time based patterns

## Next Steps

- Amazon s3 Intro
