# Amazon ECS Intro (Amazon Docs)

## Introduction

- Amazon Elastic Container Service (ECS) is a highly scalable, high performance container management service that supports Docker containers and allows you to easily run applications on a managed cluster of Amazon Elastic Compute Cloud (Amazon EC2) instances.

## Cloud Research

### Launch types

##### There are two models that you can use to run your containers:

- Fargate launch type - This is a serverless pay-as-you-go option. You can run containers without needing to manage your infrastructure.

- EC2 launch type - Configure and deploy EC2 instances in your cluster to run your containers.

##### The Fargate launch type is suitable for the following workloads:

- Large workloads that need to be optimized for low overhead

- Small workloads that have occasional burst

- Tiny workloads

- Batch workloads

##### The EC2 launch type is suitable for the following workloads:

- Workloads that require consistently high CPU core and memory usage

- Large workloads that need to be optimized for price

- Your applications need to access persistent storage

- You must directly manage your infrastructure

### Fargate

- Launch Docker containers on
  AWS
- You do not provision the
  infrastructure (no EC2 instances
  to manage)
  – simpler!
- Serverless offering
- AWS just runs containers for
  you based on the CPU / RAM
  you need

### ECR

- Elastic Container Registry
- Private Docker Registry on
  AWS
- This is where you store your
  Docker images so they can
  be run by ECS or Fargate

## Next Steps

- Intro to Serverless
