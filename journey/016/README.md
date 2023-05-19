# EBS Snapshots & EBS Snapshots Features (Udemy | Stephane Mareek)

## Introduction

EBS Snapshots are a point-in-time copy of your data, and can be used to enable disaster recovery, migrate data across regions and accounts, and improve backup compliance. You can create and manage your EBS Snapshots through the AWS Management Console, AWS Command Line Interface (CLI), or the AWS SDKs. The journey will be like this:

- EBS Snapshots
- EBS Snapshots Features

## Cloud Research

### EBS Snapshots

- Make a backup (snapshot) of your EBS volume at a point in time
- Not necessary to detach volume to do snapshot, but recommended
- Can copy snapshots across AZ or Region

### EBS Snapshots Features

#### EBS Snapshot Archive

- Move a Snapshot to an ”archive tier” that is
  75% cheaper
- Takes within 24 to 72 hours for restoring
  the archive

#### Recycle Bin for EBS Snapshots

- Setup rules to retain deleted snapshots so
  you can recover them after an accidental
  deletion
- Specify retention (from 1 day to 1 year)

## Next Steps

- Amazon Machine Image

