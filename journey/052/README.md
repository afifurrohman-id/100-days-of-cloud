# AWS Systems Manager (SSM) (Udemy | Stephane Mareek)

## Introduction

- Helps you manage your EC2 and On-Premises systems at scale
- Another Hybrid AWS service
- Get operational insights about the state of your infrastructure
- Suite of 10+ products
- Most important features are:
  > • Patching automation for enhanced compliance
  > <br>• Run commands across an entire fleet of servers
  > <br>• Store parameter configuration with the SSM Parameter Store
- Works for both Windows and Linux OS

## Cloud Research

### How Systems Manager works

- We need to install the SSM
  agent onto the systems we
  control
- Installed by default on Amazon
  Linux AMI & some Ubuntu
  AMI
- If an instance can’t be
  controlled with SSM, it’s
  probably an issue with the
  SSM agent!
- Thanks to the SSM agent, we
  can run commands, patch &
  configure our servers

### Systems Manager – SSM Session Manager

- Allows you to start a secure shell on your EC2 and
  on-premises servers
- No SSH access, bastion hosts, or SSH keys needed
- No port 22 needed (better security)
- Supports Linux, macOS, and Windows
- Send session log data to S3 or CloudWatch Logs

### AWS OpsWorks

- Chef & Puppet help you perform server configuration automatically, or
  repetitive actions
- They work great with EC2 & On-Premises VM
- AWS OpsWorks = Managed Chef & Puppet
- It’s an alternative to AWS SSM
- Only provision standard AWS resources:
  > • EC2 Instances, Databases, Load Balancers, EBS volumes…
- In the exam: Chef or Puppet needed => AWS OpsWorks

## Next Steps

- Global Infrastructure Section
