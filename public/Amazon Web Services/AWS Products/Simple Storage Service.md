---
icon: AiSimpleStorageService
aliases:
  - S3
  - Amazon S3
---
# Overview

- S3 is a key/value store for **objects**
- great for bigger objects, not so much for many small objects
- Serverless
	- scalled infinitely, max object size is 5TB
	- versioning capability
- Tiers
	- Standard
	- Infrequent access
	- Intelligent
- Feaures
	- versioning
	- encryption
	- replication
	- MFA-Delete
	- Access Logs
- Security
	- [[Identity and Access Management|IAM]]
	- Bucket Policies
	- ACL
	- Access Points
	- Object [[Lambda]]
	- CORS
	- Object/Vault Lock
		- **NEED TO KNOW IN DEPTH**
- Encryption
	- SSE-S3
	- SSe-KMS
		- can bring own kms key
	- SSE-C
	- client-side encryption
	- TLS in transit encryption
	- default encryption
- Batch Operations
	- on objects using S3 Batch
	- listing files using S3 Inventory
- Performance: 
	- Multi-part upload
	- S3 Transfer Acceleration
	- S3 Select
- Automation
	- S3 Event Notifications
		- [[Simple Notification Service|SNS]]
		- [[Simple Queue Service|SQS]]
		- [[Lambda]]
		- [[EventBridge]]
- Use cases
	- static files
	- ley value store for big files
	- website hosting
	- 

## Overview 
Amazon S3 (Simple Storage Service) is a scalable object storage service provided by AWS that allows you to store and retrieve any amount of data from anywhere on the web. It is designed to deliver 99.999999999% durability and provides a simple web services interface to store and retrieve any amount of data at any time.
## S3 Cross Region Replication 

### Pricing
- S3 ingress
	- free
- S3 to internet
	- $0.09 per GB
-  S3 Transfer Acceleration 
- #### Storage class pricing
	- S3 Standard = $.023 per GB per month

### Lifecycle transitions

Amazon S3 supports a waterfall model for transitioning between storage classes, as shown in the diagram below:
![[Pasted image 20240514120922.png]]
#### Supported lifecycle transitions
- S3 Standard to ANY other storage class
- Any storage class to the S3 Glacier or S3 Glacier Deep Archive storage classes
- S3 Standard-IA storage class to the S3 Intelligent-Tiering or S3 One Zone-IA storage classes
- The S3 Intelligent-Tiering storage class to the S3 One Zone-IA storage class
- The S3 Glacier storage class to the S3 Glacier Deep Archive storage class.

#### Unsupported lifecycle transitions
- ANY storage class to the Amazon S3 Standard storage class. 
- Any storage class to the Reduced Redundancy storage class. 
- Amazon S3 Intelligent-Tiering storage class to the Amazon S3 Standard-IA storage class. 
- The Amazon S3 One Zone-IA storage class to the Amazon S3 Standard-IA or Amazon S3 Intelligent-Tiering storage classes. 

#### Minimum storage duration for transitioning
- 30 days before transition from S3 Standard to S3 Standard-IA
- 30 days before transition from S3 Standard-IA One-Zone IA