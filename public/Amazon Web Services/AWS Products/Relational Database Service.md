---
icon: AiRDS
aliases:
  - RDS
  - Amazon RDS
---
# Relational Database Service
https://aws.amazon.com/rds/features/multi-az/

- Managed PostgreSQL/MySQL/Oracle/SQL Server/DB2/Maria DB/Custom
- RDS resources are provisioned similar to EC2
	- RDS instance size and EBS Volume type and size
	- Auto-scaling
	- Support for [[#read replica configuration|read replicas]] and [[#Multi-AZ configuration|multi-AZ]]
- Security through
	- [[Identity and Access Management|IAM]]
	- [[Security Groups]]
	- [[Key Management Service]]
	- SSl in transit
- Backup/recovery
	- Automated backup with Point in time restore
		- Up to 35 days
	- Manual snapshots for longer term recovery
- Maintenance
	- Managed and Schedule (with downtime)
- Support for IAM authentication, integration with [[Secrets Manager]]
- RDS Custom for access to and customize underlying instance (Oracle & SQL server)


## Configuration Types

### Single-AZ
- **Available engines (same as Multi-AZ with single standby)**
	- [[Relational Database Service|Amazon RDS]] for [[PostgreSQL]]
	- [[Relational Database Service|Amazon RDS]] for [[MySQL]]
	- [[Relational Database Service|Amazon RDS]] for [[MariaDB]]
	- [[Relational Database Service|Amazon RDS]] for [[SQL Server]]
	- [[Relational Database Service|Amazon RDS]] for [[Oracle Corporation|Oracle]]
	- [[Relational Database Service|Amazon RDS]] for [[IBM Db2|Db2]]
- **Additional read capacity**
	- none
		- read capacity is limited to primary 
- **Automatic failover duration**
	- Not available
		- a user-initiated point-in-time restore operation is required
			- This can take several hours
			- point-in-time restore snapshot frequency = about 5 mins 
- **Minor version upgrades downtime**
	- When using Automatic Minor Version Upgrades, minor version upgrade downtime occurs during the Amazon RDS 30-minute maintenance window
- **Higher resiliency to AZ outage**
	- none
- **Lower jitter for transaction commits**
	- no optimization for jitter
### Multi-AZ configuration
- Non-Aurora replicates synchronously 
- Aurora type replicates asynchronously

Amazon RDS Multi-AZ deployments provide enhanced availability and durability for RDS database (DB) instances, making them a natural fit for production database workloads. When you provision a Multi-AZ DB Instance, Amazon RDS automatically creates a primary DB Instance and synchronously replicates the data to a standby instance in a different Availability Zone (AZ). In case of an infrastructure failure, Amazon RDS performs an automatic failover to the standby so that you can resume database operations as soon as the failover is complete.

#### Multi-AZ with **one** standby
- **Available engines (same as single-az deployment)**
	- [[Relational Database Service|Amazon RDS]] for [[PostgreSQL]]
	- [[Relational Database Service|Amazon RDS]] for [[MySQL]]
	- [[Relational Database Service|Amazon RDS]] for [[MariaDB]]
	- [[Relational Database Service|Amazon RDS]] for [[SQL Server]]
	- [[Relational Database Service|Amazon RDS]] for [[Oracle Corporation|Oracle]]
	- [[Relational Database Service|Amazon RDS]] for [[IBM Db2|Db2]]
- **Additional Read capacity**
	- None: Your standby DB instance is only a passive failover target for high availability
- **Automatic failover duration**
	- as quickly as 60 seconds
	- failover time is independent of write throughput
- **Minor version upgrades downtime**
	- When using Automatic Minor Version Upgrades, minor version upgrade downtime occurs during the Amazon RDS 30-minute maintenance window
- **Higher resiliency to AZ outage**
	- In the event of an AZ failure, your workload will automatically failover to the up-to-date standby
- **Lower jitter for transaction commits**
	- Access to Dedicated Log Volumes
#### Multi-AZ with two readable standbys
- **Available engines**
	- 
- **Additional Read capacity**
- **Lower latency**
	- higher throughput for transaction commits
- **Automatic failover duration**
- **Minor version upgrades downtime**
- **Higher resiliency to AZ outage**
- **Lower jitter for transaction commits**

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