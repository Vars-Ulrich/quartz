---
sticker: vault//Media/icons/aws-icons/Aurora.svg
---
# Overview
Amazon Aurora is a MySQL and PostgreSQL-compatible relational database built for the cloud, that combines the performance and availability of traditional enterprise databases with the simplicity and cost-effectiveness of open source databases.


## Aurora with multi-master cluster

Amazon Aurora (Aurora) is a fully managed relational database engine that's compatible with MySQL and PostgreSQL. With some workloads, Aurora can deliver up to five times the throughput of MySQL and up to three times the throughput of PostgreSQL without requiring changes to most of your existing applications. In a multi-master cluster, all DB instances have read/write capability. Currently, all DB instances in a multi-master cluster must be in the same AWS Region. You can't enable cross-Region replicas from multi-master clusters.

### Aurora Replica
- Aurora Replicas have two main purposes.
	- Issue queries to them to scale the read operations for your application
		- Typically do so by connecting to the reader endpoint of the cluster.
			- This allows for spreading the load for read-only connections across as many Aurora Replicas as you have in the cluster.
	- Increase availability
		- If a writer instance in cluster becomes unavailable, Aurora automatically promotes one of the reader instances to take its place as a new writer
Up to 15 Aurora replicas can be distributed across the AZs that a DB cluster spans within an AWS Region
#### Exam Alerts
#saa_exam_alerts 
- If you see a sentence pertaining to sub-second cross-region replication for your database, it is a hint to use... :: Global [[Aurora]]
<!--SR:!2024-05-04,1,230-->
-  

