# Amazon API Gateway, Batch, Amazon Lightsail (Udemy | Stephane Maarek)

## Cloud Research

### Amazon API Gateway

- Fully managed service for developers to easily create, publish, maintain,
  monitor, and secure APIs
- Serverless and scalable
- Supports RESTful APIs and WebSocket APIs
- Support for security, user authentication, API throttling, API keys, monitoring...

### AWS Batch

- Fully managed batch processing at any scale
- Efficiently run 100,000s of computing batch jobs on AWS
- A “batch” job is a job with a start and an end (opposed to continuous)
- Batch will dynamically launch EC2 instances or Spot Instances
- AWS Batch provisions the right amount of compute / memory
- You submit or schedule batch jobs and AWS Batch does the rest!
- Batch jobs are defined as Docker images and run on ECS
- Helpful for cost optimizations and focusing less on the infrastructure

### Batch vs Lambda

- Lambda:

  > • Time limit
  > <br>• Limited runtimes
  > <br>• Limited temporary disk space
  > <br>• Serverless

- Batch:
  > • No time limit
  > <br>• Any runtime as long as it’s packaged as a Docker image
  > <br>• Rely on EBS / instance store for disk space
  > <br>• Relies on EC2 (can be managed by AWS)

### Amazon Lightsail

- Virtual servers, storage, databases, and networking
- Low & predictable pricing
- Simpler alternative to using EC2, RDS, ELB, EBS, Route 53…
- Great for people with little cloud experience!
- Can setup notifications and monitoring of your Lightsail resources
- Use cases:
  > • Simple web applications (has templates for LAMP, Nginx, MEAN, Node.js…)
  > <br>• Websites (templates for WordPress, Magento, Plesk, Joomla)
  > <br>• Dev / Test environment
- Has high availability but no auto-scaling, limited AWS integrations

## Next Steps

- Deploying and Managing
  Infrastructure at Scale Section
