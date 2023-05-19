# AWS CodeDeploy, AWS CodeCommit, AWS CodeBuild, AWS CodePipeline, AWS CodeArtifact, AWS CodeStar, AWS Cloud9 (Udemy | Stephane Mareek)

## Cloud Research

### AWS CodeDeploy

- We want to deploy our application
  automatically
- Works with EC2 Instances
- Works with On-Premises Servers
- Hybrid service
- Servers / Instances must be provisioned
  and configured ahead of time with the
  CodeDeploy Agent

### AWS CodeCommit

- Before pushing the application code to servers, it needs to be stored
  somewhere
- Developers usually store code in a repository, using the Git technology
- A famous public offering is GitHub, AWS’ competing product is CodeCommit
- CodeCommit:

  > • Source-control service that hosts Git-based repositories
  > <br>• Makes it easy to collaborate with others on code
  > <br>• The code changes are automatically versioned

- Benefits:
  > • Fully managed
  > <br>• Scalable & highly available
  > <br>• Private, Secured, Integrated with AWS

### AWS CodeBuild

- Code building service in the cloud (name is obvious)
- Compiles source code, run tests, and produces packages that are ready to be
  deployed (by CodeDeploy for example)
- Benefits:
  > • Fully managed, serverless
  > <br>• Continuously scalable & highly available
  > <br>• Secure
  > <br>• Pay-as-you-go pricing – only pay for the build time

### AWS CodePipeline

- Orchestrate the different steps to have the code automatically pushed to production

  > • Code => Build => Test => Provision => Deploy
  > <br>• Basis for CICD (Continuous Integration & Continuous Delivery)

- Benefits:
  > • Fully managed, compatible with CodeCommit, CodeBuild, CodeDeploy, Elastic Beanstalk,
  > CloudFormation, GitHub, 3rd-party services (GitHub…) & custom plugins…
  > <br>• Fast delivery & rapid updates

### AWS CodeArtifact

- Software packages depend on each other to be built (also called code
  dependencies), and new ones are created
- Storing and retrieving these dependencies is called artifact management
- Traditionally you need to setup your own artifact management system
- CodeArtifact is a secure, scalable, and cost-effective artifact
  management for software development
- Works with common dependency management tools such as Maven,
  Gradle, npm, yarn, twine, pip, and NuGet
- Developers and CodeBuild can then retrieve dependencies straight from CodeArtifact

### AWS CodeStar

- Unified UI to easily manage software development activities in one place
- “Quick way” to get started to correctly set-up CodeCommit, CodePipeline,
  CodeBuild, CodeDeploy, Elastic Beanstalk, EC2, etc…
- Can edit the code ”in-the-cloud” using AWS Cloud9

### AWS Cloud9

- AWS Cloud9 is a cloud IDE (Integrated
  Development Environment) for writing, running
  and debugging code
- “Classic” IDE (like IntelliJ, Visual Studio Code…)
  are downloaded on a computer before being
  used
- A cloud IDE can be used within a web browser,
  meaning you can work on your projects from
  your office, home, or anywhere with internet
  with no setup necessary
- AWS Cloud9 also allows for code collaboration
  in real
  -time (pair programming)

## Next Steps

- Meet 6 | EBS, AMI
