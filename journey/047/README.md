# Deploying and Managing Infrastructure at Scale Section (Udemy | Stephane Mareek)

## Cloud Research

### What is CloudFormation

- CloudFormation is a declarative way of outlining your AWS
  Infrastructure, for any resources (most of them are supported).
- For example, within a CloudFormation template, you say:
  > • I want a security group
  > <br>• I want two EC2 instances using this security group
  > <br>• I want an S3 bucket
  > <br>• I want a load balancer (ELB) in front of these machines
- Then CloudFormation creates those for you, in the right order, with the
  exact configuration that you specify

### Benefits of AWS CloudFormation

- Infrastructure as code

  > • No resources are manually created, which is excellent for control
  > <br>• Changes to the infrastructure are reviewed through code

- Cost

  > • Each resources within the stack is tagged with an identifier so you can easily see how
  > much a stack costs you
  > <br>• You can estimate the costs of your resources using the CloudFormation template
  > <br>• Savings strategy: In Dev, you could automation deletion of templates at 5 PM and
  > recreated at 8 AM, safely

- Productivity

  > • Ability to destroy and re-create an infrastructure on the cloud on the fly
  > <br>• Automated generation of Diagram for your templates!
  > <br>• Declarative programming (no need to figure out ordering and orchestration)

- Don’t re-invent the wheel

  > • Leverage existing templates on the web!
  > <br>• Leverage the documentation

- Supports (almost) all AWS resources:
  > • Everything we’ll see in this course is supported
  > <br>• You can use “custom resources” for resources that are not supported

### AWS Cloud Development Kit (CDK)

- Define your cloud infrastructure using a familiar language:
  > • JavaScript/TypeScript, Python, Java, and .NET
- The code is “compiled” into a CloudFormation template (JSON/YAML)
- You can therefore deploy infrastructure and application runtime code together
  > • Great for Lambda functions
  > <br>• Great for Docker containers in ECS / EKS

### Developer problems on AWS

- Managing infrastructure
- Deploying Code
- Configuring all the databases, load balancers, etc
- Scaling concerns
- Most web apps have the same architecture (ALB + ASG)
- All the developers want is for their code to run!
- Possibly, consistently across different applications and environments

## Next Steps

- AWS Elastic Beanstalk
