---
sticker: vault//Media/icons/aws-icons/RDS.svg
aliases:
  - RDS
---
# RDS (Relational Database Service)
https://aws.amazon.com/rds/features/multi-az/

## Configuration Types
### Multi-AZ configuration

enhanced database availability

Non-Aurora replicates synchronously 
Aurora type replicates asynchronously

Amazon RDS Multi-AZ deployments provide enhanced availability and durability for RDS database (DB) instances, making them a natural fit for production database workloads. When you provision a Multi-AZ DB Instance, Amazon RDS automatically creates a primary DB Instance and synchronously replicates the data to a standby instance in a different Availability Zone (AZ). In case of an infrastructure failure, Amazon RDS performs an automatic failover to the standby so that you can resume database operations as soon as the failover is complete.

### Multi-Region configuration

### read replica configuration

main purpose is scalability

replicates asynchronously

can be single AZ, Cross-AZ, or Cross Region 

![[Pasted image 20240514151022.png]]
## RDS Custom
#### RDS Custom for Oracle
- allows access to and customization of your underlying database server hose and OS

https://aws.amazon.com/blogs/aws/amazon-rds-custom-for-oracle-newcontrol-capabilities-in-database-environment/
#### RDS Custom for SQL Server