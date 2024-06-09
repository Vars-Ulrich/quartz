---
icon: AiRDS
aliases:
  - RDS
  - Amazon RDS
  - Amazon Relation Database Service
---
# Relational Database Service
https://aws.amazon.com/rds/features/multi-az/
## Overview

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

### Single-AZ Configuration
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
#### Multi-AZ with **one** standby
##### Specifics
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
	- 
##### How it works
- In an Amazon RDS Multi-AZ deployment, Amazon RDS automatically creates a primary database (DB) instance and synchronously replicates the data to an instance in a different AZ. When it detects a failure, Amazon RDS automatically fails over to a standby instance without manual intervention.
- ![[How multi-az single standby works.png]]

#### Multi-AZ with two readable standbys
##### Specifics
- **Available engines**
	- [[Relational Database Service|Amazon RDS]] for [[PostgreSQL]]
	- [[Relational Database Service|Amazon RDS]] for [[MySQL]]
- **Additional Read capacity**
	- Two standby DB instances act as failover targets and serve read traffic
	- Read capacity is determined by the overhead of write transactions from the primary
- **Lower latency**
	- higher throughput for transaction commits
	- Up to 2x faster transaction commits compared to Amazon RDS Multi-AZ with one standby
- **Automatic failover duration**
	- A new primary is available to serve your new workload in typically under 35 seconds
	- Failover time depends on length of replica lag
- **Minor version upgrades downtime**
	- Typically under 1 second **when customers add an open source or Amazon RDS Proxy** to their deployment
	- Typically under 35 seconds with Multi-AZ with two readable standbys alone
- **Higher resiliency to AZ outage**
	- In the event of a failure, one of the two remaining standbys will takeover and serve the workload (writes) from the primary
- **Lower jitter for transaction commits**
	- Uses local storage for transactional logs to reduce jitter

##### How it works
Deploy highly available, durable MySQL or PostgreSQL databases in three AZs using Amazon RDS Multi-AZ with two readable standbys. Gain automatic failovers in typically under 35 seconds, up to 2x faster transaction commit latency compared to Amazon RDS Multi-AZ with one standby, additional read capacity, and a choice of AWS Graviton2– or Intel–based instances for compute.
- ![[How multi-az with two standbys works.png]]


#### Pricing
For Single-AZ deployments, Multi-AZ deployments with one standby instance, and Multi-AZ deployments with two readable standbys, pricing is per DB instance-hour consumed, from the time a DB instance is launched until it is stopped or deleted. Partial DB instance-hours are billed in one-second increments with a 10 minute minimum charge following a billable status change such as creating, starting, or modifying the DB instance class.

##### Specifics
- **Available engines**
	- [[Relational Database Service|Amazon RDS]] for [[PostgreSQL]]
	- [[Relational Database Service|Amazon RDS]] for [[MySQL]]
- **Additional Read capacity**
	- Two standby DB instances act as failover targets and serve read traffic
	- Read capacity is determined by the overhead of write transactions from the primary
- **Lower latency**
	- higher throughput for transaction commits
	- Up to 2x faster transaction commits compared to Amazon RDS Multi-AZ with one standby
- **Automatic failover duration**
	- A new primary is available to serve your new workload in typically under 35 seconds
	- Failover time depends on length of replica lag
- **Minor version upgrades downtime**
	- Typically under 1 second **when customers add an open source or Amazon RDS Proxy** to their deployment
	- Typically under 35 seconds with Multi-AZ with two readable standbys alone
- **Higher resiliency to AZ outage**
	- In the event of a failure, one of the two remaining standbys will takeover and serve the workload (writes) from the primary
- **Lower jitter for transaction commits**
	- Uses local storage for transactional logs to reduce jitter

##### How it works
Deploy highly available, durable MySQL or PostgreSQL databases in three AZs using Amazon RDS Multi-AZ with two readable standbys. Gain automatic failovers in typically under 35 seconds, up to 2x faster transaction commit latency compared to Amazon RDS Multi-AZ with one standby, additional read capacity, and a choice of AWS Graviton2– or Intel–based instances for compute.
- ![[How multi-az with two standbys works.png]]


##### Customers
###### SysCloud
SysCloud creates automatic backups for critical software as a service (SaaS) applications, monitors for malicious files, and delivers powerful insights about your data and compliance —all from one dashboard. SysCloud uses Amazon RDS Multi-AZ with two readable standbys for its internal monitoring system: “The new Amazon RDS Multi-AZ deployment option offers us a cost-efficient way to achieve better performance, availability, and read scalability,” said Vikram Srinivasan, Director, Infrastructure at SysCloud. “With the new Amazon RDS Multi-AZ deployment option, we expect to create a better experience for our customers.”

### Multi-Region configuration
### read replica configuration
- main purpose is scalability
- replicates asynchronously
- can be single AZ, Cross-AZ, or Cross Region 

![[Pasted image 20240514151022.png]]

## RDS Custom
#### RDS Custom for Oracle
- allows access to and customization of your underlying database server hose and OS

https://aws.amazon.com/blogs/aws/amazon-rds-custom-for-oracle-newcontrol-capabilities-in-database-environment/
#### RDS Custom for SQL Server