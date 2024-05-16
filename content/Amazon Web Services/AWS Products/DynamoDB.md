---
sticker: vault//Media/icons/aws-icons/DynamoDB.svg
---
a key-value and document database that delivers single-digit millisecond performance at any scale. It's a fully managed, multi-Region, multi-master, durable database with built-in security, backup and restore, and in-memory caching for internet-scale applications.
Support high availability by default

- AWS proprietary technology
- managed serverless NoSQL database
- millisecond latency (microsecond with [[#Dynamo DB accelerator (DAX)|DAX]])
- Capacity modes
	- **privsioned** capacity with optional auto-scaling
	- on-demand capacity
- Can replace [[ElastiCache]] as a key/value store 
	- for example, storing session data, using [[Time to live|TTL]] feature
- Highly available
	- multi-AZ by default
	- read and writes are decoupled
	- transaction capability
- DAX cluster for read cache
	- microsecond read latency
- Security, authentication, and authorization
	- all done through [[Identity and Access Management|IAM]]
- Event Processing
	- [[#Dynamo DB Streams]] to integrate with 
		- [[Lambda]]
			- Can be invoked for **every** change in your DynamoDB table
		- [[Kinesis Data Streams]]
- [[#DynamoDB w/ global tables|Global Table Feature]]
	- [[active-active setup]]
- Backup options
	- Automated backups
		- up to 3 days with PITR
			- restore to new table
	- On-demand backups
- Export to [[Simple Storage Service|S3]]
	- without using RCU within the PITR window
- Import form [[Simple Storage Service|S3]]
	- without using WCU
- Use Case: 
	- Serverless applications development
		- **small docs** 100s KB
		- distributed serverless cache


## DynamoDB w/ global tables

Amazon DynamoDB is a fully managed, serverless, key-value NoSQL database designed to run high-performance applications at any scale. DynamoDB offers built-in security, continuous backups, automated multi-region replication, in-memory caching, and data export tools.

DynamoDB global tables replicate data automatically across your choice of AWS Regions and automatically scale capacity to accommodate your workloads. With global tables, your globally distributed applications can access data locally in the selected regions to get single-digit millisecond read and write performance. DynamoDB offers active-active cross-region support that is needed for the company.

## Dynamo DB accelerator (DAX)

## Dynamo DB Streams


#### Exam Alerts 
#saa_exam_alerts 
- Any time that you see that you need to rapidly evolve schemas/have a flexible type of database schema, a great choice would be... :: [[DynamoDB]]
<!--SR:!2024-05-04,1,230-->


##### Key words
- Schemaless