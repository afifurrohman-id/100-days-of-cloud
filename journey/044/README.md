# Serverless Intro (Udemy | Stephane Mareek)

## Cloud Research

### What’s serverless?

- Serverless is a new paradigm in which the developers don’t have to
  manage servers anymore…
- They just deploy code
- They just deploy… functions !
- Initially... Serverless == FaaS (Function as a Service)
- Serverless was pioneered by AWS Lambda but now also includes
  anything that’s managed: “databases, messaging, storage, etc.”
- Serverless does not mean there are no servers…
  it means you just don’t manage / provision / see them

### What is AWS Lambda

AWS Lambda is a compute service that lets you run code without provisioning or managing servers. Lambda runs your code on a high-availability compute infrastructure and performs all of the administration of the compute resources, including server and operating system maintenance, capacity provisioning and automatic scaling, and logging. With Lambda, you can run code for virtually any type of application or backend service. All you need to do is supply your code in one of the languages that Lambda supports.

You organize your code into Lambda functions. Lambda runs your function only when needed and scales automatically, from a few requests per day to thousands per second. You pay only for the compute time that you consume—there is no charge when your code is not running

### Why AWS Lambda

##### EC2

- Virtual Servers in the Cloud
- Limited by RAM and CPU
- Continuously running
- Scaling means intervention to add / remove servers

##### Amazon Lambda

- Virtual functions – no servers to manage!
- Limited by time - short executions
- Run on-demand
- Scaling is automated!

### Benefits of AWS Lambda

- Easy Pricing:
  > • Pay per request and compute time
  > <br>• Free tier of 1,000,000 AWS Lambda requests and 400,000 GBs of compute time
- Integrated with the whole AWS suite of services
- Event-Driven: functions get invoked by AWS when needed
- Integrated with many programming languages
- Easy monitoring through AWS CloudWatch
- Easy to get more resources per functions (up to 10GB of RAM!)
- Increasing RAM will also improve CPU and network

### AWS Lambda language support

- Node.js (JavaScript)
- Python
- Java (Java 8 compatible)
- C# (.NET Core)
- Golang
- C# / Powershell
- Ruby
- Custom Runtime API (community supported, example Rust)
- Lambda Container Image
  > • The container image must implement the Lambda Runtime API
  > <br>• ECS / Fargate is preferred for running arbitrary Docker images

### AWS Lambda Pricing: example

- You can find overall pricing information here:
  > https://aws.amazon.com/lambda/pricing/
- Pay per calls
  :
  > • First 1,000,000 requests are free
  > <br>• $0.20 per 1 million requests thereafter ($0.0000002 per request)
- Pay per duration: (in increment of 1 ms
  )
  > • 400,000 GB
  > -seconds of compute time per month for FREE
  > <br>• == 400,000 seconds if function is 1GB RAM
  > <br>• == 3,200,000 seconds if function is 128 MB RAM
  > <br>• After that $1.00 for 600,000 GB-seconds
- It is usually very cheap to run AWS Lambda so it’s very popular

## Next Steps

- Meet 5 | EC2 Instance Web Server & SSH
