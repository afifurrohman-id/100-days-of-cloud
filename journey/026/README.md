# Amazon S3 – Static Website Hosting, Amazon S3 - Versioning, Amazon S3 – Replication (CRR & SRR) (Udemy | Stephane Mareek)

## Cloud Research

### Amazon S3 – Static Website Hosting

- S3 can host static websites and have them accessible on
  the Internet
- The website URL will be (depending on the region)
  > • http://bucket-name.s3-website-aws-region.amazonaws.com
  > OR
  > <br>• http://bucket-name.s3-website.aws-region.amazonaws.com
- If you get a 403 Forbidden error, make sure the bucket
  policy allows public reads!

### Amazon S3 - Versioning

- You can version your files in Amazon S3
- It is enabled at the bucket level
- Same key overwrite will change the “version”: 1, 2, 3….
- It is best practice to version your buckets
  > • Protect against unintended deletes (ability to restore a version)
  > <br>• Easy roll back to previous version
- Notes:
  > • Any file that is not versioned prior to enabling versioning will
  > have version “null”
  > <br>• Suspending versioning does not delete the previous versions

### Amazon S3 – Replication (CRR & SRR)

- Must enable Versioning in source and destination buckets
- Cross-Region Replication (CRR)
- Same-Region Replication (SRR)
- Buckets can be in different AWS accounts
- Copying is asynchronous
- Must give proper IAM permissions to S3
- Use cases:
  > • CRR – compliance, lower latency access, replication across accounts
  > <br>• SRR – log aggregation, live replication between production and test
  > accounts

## Next Steps

- S3 Storage Classes
