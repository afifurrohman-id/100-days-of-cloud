# Amazon S3 Intro (Udemy | Stephane Mareek)

## Introduction

- Amazon S3 is one of the main building blocks of AWS
- It’s advertised as ”infinitely scaling” storage
- Many websites use Amazon S3 as a backbone
- Many AWS services use Amazon S3 as an integration as well
- We’ll have a step-by-step approach to S3

## Cloud Research

### Amazon S3 - Buckets

- Amazon S3 allows people to store objects (files) in “buckets” (directories)
- Buckets must have a globally unique name (across all regions all accounts)
- Buckets are defined at the region level
- S3 looks like a global service but buckets are created in a region
- Naming convention
  > • No uppercase, No underscore
  > <br>• 3-63 characters long
  > <br>• Not an IP
  > <br>• Must start with lowercase letter or number
  > <br>• Must NOT start with the prefix xn--
  > <br>• Must NOT end with the suffix -s3alias

### Amazon S3 - Objects

- Objects (files) have a Key
- The key is the FULL path:
- s3://my-bucket/my_file.txt
- s3://my-bucket/my_folder1/another_folder/my_file.txt
- The key is composed of prefix + object name
- s3://my-bucket/my_folder1/another_folder/my_file.txt
- There’s no concept of “directories” within buckets
  (although the UI will trick you to think otherwise)
- Just keys with very long names that contain slashes (“/”)

### Amazon S3 – Objects (cont.)

- Object values are the content of the body:
  > • Max. Object Size is 5TB (5000GB)
  > <br>• If uploading more than 5GB, must use “multi-part upload”
- Metadata (list of text key / value pairs – system or user metadata)
- Tags (Unicode key / value pair – up to 10) – useful for security / lifecycle
- Version ID (if versioning is enabled)

## Next Steps

- Amazon S3 – Security
