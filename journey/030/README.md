# AWS OpsHub, Hybrid Cloud for Storage, AWS Storage Gateway (Udemy | Stephane Mareek)

## Cloud Research

### AWS OpsHub

- Historically, to use Snow Family devices, you
  needed a CLI (Command Line Interface tool)
- Today, you can use AWS OpsHub (a software you install on your computer / laptop) to
  manage your Snow Family Device
  > • Unlocking and configuring single or clustered devices
  > <br>• Transferring files
  > <br>• Launching and managing instances running on Snow
  > Family Devices
  > <br>• Monitor device metrics (storage capacity, active
  > instances on your device)
  > <br>• Launch compatible AWS services on your devices
  > (ex: Amazon EC2 instances, AWS DataSync, Network File System (NFS))

### Hybrid Cloud for Storage

- AWS is pushing for ”hybrid cloud”
  > • Part of your infrastructure is on-premises
  > <br>• Part of your infrastructure is on the cloud
- This can be due to
  > • Long cloud migrations
  > <br>• Security requirements
  > <br>• Compliance requirements
  > <br>• IT strategy
- S3 is a proprietary storage technology (unlike EFS / NFS), so how do you
  expose the S3 data on-premise?
- AWS Storage Gateway!

### AWS Storage Gateway

- Bridge between on-premise data and cloud
  data in S3
- Hybrid storage service to allow on- premises to seamlessly use the AWS Cloud
- Use cases: disaster recovery, backup &
  restore, tiered storage
- Types of Storage Gateway:
  > • File Gateway
  > <br>• Volume Gateway
  > <br>• Tape Gateway
- No need to know the types at the exam

## Next Steps

- Databases Section
