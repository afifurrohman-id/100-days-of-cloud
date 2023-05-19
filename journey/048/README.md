# AWS Elastic Beanstalk (Udemy | Stephane Mareek)

## Introduction

- Elastic Beanstalk is a developer centric view of deploying
  an application on AWS
- It uses all the component’s we’ve seen before:
  EC2, ASG, ELB, RDS, etc…
- But it’s all in one view that’s easy to make sense of!
- We still have full control over the configuration
- Beanstalk = Platform as a Service (PaaS)
- Beanstalk is free but you pay for the underlying instances

## Cloud Research

### Elastic Beanstalk

- Managed service

  > • Instance configuration / OS is handled by Beanstalk
  > <br>• Deployment strategy is configurable but performed by Elastic Beanstalk
  > <br>• Capacity provisioning
  > <br>• Load balancing & auto-scaling
  > <br>• Application health-monitoring & responsiveness

- Just the application code is the responsibility of the developer

- Three architecture models:

  > • Single Instance deployment: good for dev
  > <br>• LB + ASG: great for production or pre-production web applications
  > <br>• ASG only: great for non-web apps in production (workers, etc..)

- Support for many platforms:
  > • Go
  > <br>• Java SE
  > <br>• Java with Tomcat
  > <br>• .NET on Windows Server with IIS
  > <br>• Node.js
  > <br>• PHP
  > <br>• Python
  > <br>• Ruby
  > <br>• Packer Builder
  > <br>• Single Container Docker
  > <br>• Multi-Container Docker
  > <br>• Preconfigured Docker
- If not supported, you can write
  your custom platform (advanced)

## Next Steps

- AWS CodeDeploy, AWS CodeCommit, AWS CodeBuild, AWS CodePipeline, AWS CodeArtifact, AWS CodeStar, AWS Cloud9
