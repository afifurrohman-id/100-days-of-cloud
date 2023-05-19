# AWS RDS (Udemy | Stephane Mareek)

## Introduction

- RDS stands for Relational Database Service
- It’s a managed DB service for DB use SQL as a query language.
- It allows you to create databases in the cloud that are managed by AWS
  > • Postgres
  > <br>• MySQL
  > <br>• MariaDB
  > <br>• Oracle
  > <br>• Microsoft SQL Server
  > <br>• Aurora (AWS Proprietary database)

## Cloud Research

### Advantage over using RDS versus deploying

DB on EC2

- RDS is a managed service:
  > • Automated provisioning, OS patching
  > <br>• Continuous backups and restore to specific timestamp (Point in Time Restore)!
  > <br>• Monitoring dashboards
  > <br>• Read replicas for improved read performance
  > <br>• Multi AZ setup for DR (Disaster Recovery)
  > <br>• Maintenance windows for upgrades
  > <br>• Scaling capability (vertical and horizontal)
  > <br>• Storage backed by EBS (gp2 or io1)
- BUT you can’t SSH into your instances

### Amazon Aurora

- Aurora is a proprietary technology from AWS (not open sourced)
- PostgreSQL and MySQL are both supported as Aurora DB
- Aurora is “AWS cloud optimized” and claims 5x performance improvement
  over MySQL on RDS, over 3x the performance of Postgres on RDS
- Aurora storage automatically grows in increments of 10GB, up to 64 TB.
- Aurora costs more than RDS (20% more) – but is more efficient
- Not in the free tier

### RDS Deployments: Read Replicas, Multi-AZ

- Read Replicas:

  > • Scale the read workload of your DB
  > <br>• Can create up to 5 Read Replicas
  > <br>• Data is only written to the main DB

- Multi-AZ:
  > • Failover in case of AZ outage (high availability)
  > <br>• Data is only read/written to the main database
  > <br>• Can only have 1 other AZ as failover

### RDS Deployments: Multi-Region

- Multi-Region (Read Replicas)
  > • Disaster recovery in case of region issue
  > <br>• Local performance for global reads
  > <br>• Replication cost

## Next Steps

- Amazon ElastiCache
