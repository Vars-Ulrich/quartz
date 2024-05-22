---
icon: AiEMR
aliases:
- EMR
---
# Overview

The industry-leading cloud big data platform for processing vast amounts of data using open source tools such as [[Apache Hadoop|Hadoop]], Apache Spark, Apache Hive, Apache HBase, Apache Flink, Apache Hudi, and Presto. Amazon EMR can be used to provision resources to run big data workloads on Hadoop clusters. EMR provisions EC2 instances to manage its workload. EMR is not a serverless service.

- EMR helps in creating Hadoop clusters to analyze and process vast amounts of data
	- Clusters can be made of **hundreds of [[Elastic Cloud Compute|EC2]]** instances
- EMR comes bundled with:
	- Apache Spark
	- HBase
	- Presto
	- Flink
- EMR take care of all the provisioning and configuration
- Auto-scaling and integrated with Spot instances

## Use Cases
- Data processing
- machine learning
- web indexing
- big data

## Node types and purchasing
- Master node (long-running)
	- Manage the cluster
	- coordinate
	- manage health
- Core node (long-running)
	- run tasks
	- store data
- Task node (optional, usually spot instances)
	- Just to run tasks
- Purchasing options
	- on-demand
		- reliable
		- predictable
		- wont be terminated
	- reserved
		- EMR will automatically use if available
	- Spot instances
		- cheaper
		- less reliable
		- can be terminated
		- wise to leverage this on task nodes
- Deployment
	- Long running clusters
	- Transient (temporary) clusters
## ChatGPT Overview