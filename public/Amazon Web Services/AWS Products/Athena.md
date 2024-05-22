---
icon: AiAthena
aliases:
- Amazon Athena
---
# Overview

-  Amazon Athena is an interactive query service
- makes it easy to analyze data in Amazon [[Simple Storage Service|S3]] using standard [[Structured Query Language|SQL]]. 
- Athena is **serverless**, so there is no infrastructure to manage
- you pay only for the queries that you run. 
- Athena is **used for analytics** and **not to prepare** data for analytics.
- Athena supports many formats
	- CSV
	- JSON
	- ORC
	- Avro
	- Parquet
	- Possibly others
- Amazon is commonly used with [[QuickSight]] for reporting/dashboards

## Pricing
- Fixed amount
	- $5.00 per TB of data scanned

## Use Cases
- Business intelligence
- Analytics
- report, analyze, & query VPC flow logs
- [[Elastic Load Balancing|ELB]] Logs
- [[CloudTrail]] trails
- Ad-hoc queries
- Pretty much query any logs that originate from your 

## Performance Improvement

### Use **columnar data** for cost-savings (scan less!!!)
- [[Apache Parquet]] or [[Apache ORC|ORC]] is recommended.
- This is going to give you a huge performance improvement
- Use [[Glue]] to convert your data to [[Apache Parquet]] or [[Apache ORC|ORC]]

### Compress Data for smaller retrievals
- bzip2
- gzip
- lz4
- snappy
- zlip
- zstd

### Partition Datasets in S3 for Easier Querying on Virtutal Columns
- basic formatting idea
```
	s3://yourBucket/pathToTable
		/<PARTITION_COLUMN_NAME>=<VALUE>
		  /<PARTITION_COLUMN_NAME>=<VALUE>
		    /<PARTITION_COLUMN_NAME>=<VALUE>
		      /etc...
```
- example:
	```
	s3://athena-examples/flight/parquet/year=1991/month=1/day=1/
	```

### Use Larger Files to Minimize Overhead
- 128 MB or larger

## Federated Query
- Allows you to run [[Structured Query Language|SQL]] queries across data stored in relational, nne-relational, object, and custom data sources
	- AWS or om-premises
- Uses Data Source Connectors that run on [[Lambda|AWS Lambda]] to run Federated Queries, for example
	- [[CloudWatch]] Logs
	- [[DynamoDB]]
	- [[Relational Database Service|RDS]]
- Store the results back in [[Simple Storage Service|S3]]
 
## Exam Alerts
- Analyze data in [[Simple Storage Service|S3]] using serverless [[Structured Query Language|SQL]], you should be thinking [[Athena]]
- 






