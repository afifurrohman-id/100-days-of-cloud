# Amazon S3 – Security (Udemy | Stephane Mareek)

## Cloud Research

### Amazon S3 – Security

- User-Based
  > • IAM Policies – which API calls should be allowed for a specific user from IAM
- Resource-Based
  > • Bucket Policies – bucket wide rules from the S3 console - allows cross account
  > <br>• Object Access Control List (ACL) – finer grain (can be disabled)
  > <br>• Bucket Access Control List (ACL) – less common (can be disabled)
- Note: an IAM principal can access an S3 object if
  > • The user IAM permissions ALLOW it OR the resource policy ALLOWS it
  > <br>• AND there’s no explicit DENY
- Encryption: encrypt objects in Amazon S3 using encryption keys

### S3 Bucket Policies

- JSON based policies

  > • Resources: buckets and objects
  > <br>• Effect: Allow / Deny
  > <br>• Actions: Set of API to Allow or Deny
  > <br>• Principal: The account or user to apply the
  > policy to<br>

- Use S3 bucket for policy to:
  > • Grant public access to the bucket <br>• Force objects to be encrypted at upload <br>• Grant access to another account (Cross
  > Account)

## Next Steps

- Amazon S3 – Static Website Hosting, Amazon S3 -Versioning, Amazon S3 – Replication (CRR & SRR)
