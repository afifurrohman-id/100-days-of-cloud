# Amazon QLDB, Amazon Managed Blockchain, AWS Glue (Udemy | Stephane Mareek)

## Cloud Research

### Amazon QLDB

- QLDB stands for ”Quantum Ledger Database”
- A ledger is a book recording financial transactions
- Fully Managed, Serverless, High available, Replication across 3 AZ
- Used to review history of all the changes made to your application data over time
- Immutable system: no entry can be removed or modified, cryptographically verifiable
- 2-3x better performance than common ledger blockchain frameworks, manipulate data using SQL
- Difference with Amazon Managed Blockchain: no decentralization component, in accordance with

### Amazon Managed Blockchain

- Blockchain makes it possible to build applications where multiple parties
  can execute transactions without the need for a trusted, central
  authority.
- Amazon Managed Blockchain is a managed service to:
  > • Join public blockchain networks
  > <br>• Or create your own scalable private network
- Compatible with the frameworks Hyperledger Fabric & Ethereum

### AWS Glue

- Managed extract, transform, and load (ETL) service
- Useful to prepare and transform data for analytics
- Fully serverless service
- Glue Data Catalog: catalog of datasets
  > • can be used by Athena, Redshift, EMR

## Next Steps

- DMS – Database Migration Service
