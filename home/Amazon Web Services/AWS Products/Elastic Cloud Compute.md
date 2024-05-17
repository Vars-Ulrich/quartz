---
sticker: vault//Media/icons/aws-icons/EC2.svg
aliases:
  - EC2
icon:
---

- EC2 is a web service that provides secure, resizable compute capacity in the cloud with support for per-second billing. It is the easiest way to provision servers on AWS Cloud and access the underlying OS. EC2 is not a serverless service.
## EC2 User Data
- Script for bootstrapping 
- Runs only **once** at the instances first boot
- used to automate boot tasks
	- Installing updates
	- Installing software
	- Downloading common files from internet
	- anything you can think of
- Runs with the root user (sudo) privileges
## Naming Conventions
- example: m5.2xlarge
	- "m" denotes the instance class
	- "5" denotes the generation (AWS improves over time)
	- "2xlarge" denotes size within the instance class

## Instance types
### General purpose
- Great for diversity of workloads such as... 
	- Web servers
	- Code repos
- Balance between 
	- Compute
	- Memory
	- Networking
### Compute optimized
- Great for compute-intensive tasks requiring high performance processors
	- Batch proccessing workloads
	- Media transcoding
	- High performance web servers
	- HPC
	- Scientific modeling and ML
	- Dedicated gaming servers
	- will have a name beginning with C
### Memory optimized
- Fast performance for workloads that process large data sets in memory
	- HP databases, both relational and non-relational
	- Distributed web scale cache stores
	- In-mem databases optimized for Bi (business intelligence)
	- Applications performing real-time processing of big unstructured data
	- Will have names begging with "R" 
		- also "X,"  "High Memory" and "z"
			- not required knowledge for SAA
### Accelerated computing
### Storage optimized
- Storage-intensive tasks that require high, sequential r/w access to large data sets on local storage
	- High frequency online transaction processing (OLTP) systems
	- Relations and NoSQL databases
	- Cache for in-memory databases (for example, Redis)
	- Data warehousing applications
	- Distributed file systems
	- names will start with "i," "d," or "h"
### HPC optimized


## EC2 Instance Store

- An instance store provides ***temporary block-level storage*** for your EC2 instance. This storage is located on disks that are ***physically attached*** to the host computer. Instance store is ideal for the temporary storage of information that changes frequently, such as buffers, caches, scratch data, and other temporary content, or for data that is replicated across a fleet of instances, such as a load-balanced pool of web servers. Instance storage is temporary, data is lost if instance experiences failure or is terminated. EC2 instance store cannot be used for file sharing between instances.