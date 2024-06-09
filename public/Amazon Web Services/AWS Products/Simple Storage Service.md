---
icon: AiSimpleStorageService
aliases:
  - S3
  - Amazon S3
---
[**Official AWS S3 page:**](https://aws.amazon.com/s3/)
## Overview 
Amazon S3 (Simple Storage Service) is a scalable object storage service provided by AWS that allows you to store and retrieve any amount of data from anywhere on the web. It is designed to deliver 99.999999999% durability and provides a simple web services interface to store and retrieve any amount of data at any time.

- S3 is a key/value store for **objects**
	- great for bigger objects, not so much for many small objects
- Serverless
	- scaled infinitely, max object size is 5TB
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
		- can bring own [[Key Management Service|KMS]] key
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
	- key value store for big files
	- website hosting
		- redirect ability contained therein
## S3 Storage Classes
### S3 Standard
### S3 Standard-IA
### S3 Intelligent Tiering
### S3 Express One-Zone
### S3 Glacier Instant Retrieval
### S3 Glacier Flexible Retrieval
### S3 Glacier Deep Archive
### S3 One Zone - IA
## S3 Cross Region Replication 

## S3 Transfer Acceleration
Amazon S3 Transfer Acceleration can speed up content transfers to and from Amazon S3 by as much as 50-500% for long-distance transfer of larger objects. Customers who have either web or mobile applications with widespread users or applications hosted far away from their S3 bucket can experience long and variable upload and download speeds over the Internet. S3 Transfer Acceleration (S3TA) reduces the variability in Internet routing, congestion and speeds that can affect transfers, and logically shortens the distance to S3 for remote applications. S3TA improves transfer performance by routing traffic through Amazon CloudFront’s globally distributed Edge Locations and over AWS backbone networks, and by using network protocol optimizations. You can turn on S3TA with a few clicks in the S3 console, and test its benefits from your location with [a speed comparison tool](http://s3-accelerate-speedtest.s3-accelerate.amazonaws.com/en/accelerate-speed-comparsion.html). With S3TA, you pay only for transfers that are accelerated.
## Pricing


### Data Transfer Pricing (section incomplete)

#### Pricing for [[Simple Storage Service|S3]] ingress **from** internet
- always free

#### Pricing for [[Simple Storage Service|S3]] egress **to** internet
- **Free for the first 100 GB out per month**.  After that, t follows tiered pricing, with discounts being rewarded by tiers:
	- **First 10 TB/Month**
		- $0.09 per GB
	- **Next 40 TB/Month**
		- $0.085 per GB
	- **Next 100 TB/Month**
		- $0.07 per GB
	- **Greater than 150 TB/Month**
		- $0.05 per GB


#### Pricing for S3TA ingress from net
- ##### Accelerated by AWS Edge Locations in the United States, Europe, and Japan
	- **$0.04 per GB**
- ##### Accelerated by all other AWS Edge Locations
	- **$0.08 per GB**

#### Pricing for S3TA egress to net
- ##### Accelerated by any AWS Edge Location
	- **$0.04 per GB**

#### Data Transfer between Amazon S3 and another AWS region:
- ##### Accelerated by any AWS Edge Location 
	- **$0.04**

#### For Data Transfers exceeding 500 TB/Month
- Contact AWS
### Per class pricing 
(uses us-east-1 guidelines)
#### S3 Standard Pricing
- First 50 TB / Month
	- $0.023 per GB
- Next 450 TB / Month
	- $0.022 per GB
- Over 500 TB / Month
	- $0.021 per GB

#### S3 Standard IA Pricing
- All Storage / Month	
	- $0.0125 per GB

#### S3-Intelligent tiering Pricing
##### Monitoring and Automation
- All Storage / Month (Objects > 128 KB)
	- $0.0025 per 1,000 objects

##### Frequent Access Tier
Shares the same pricing with  S3 Standard
- First 50 TB / Month
	- $0.023 per GB
- Next 450 TB / Month
	- $0.022 per GB
- Over 500 TB / Month
	- $0.021 per GB

##### Infrequent Access Tier
Half the cost of FA Tier!!!

- All Storage / Month
	- $0.0125 per GB
##### Archive Instant Access Tier 
Over 80% cheaper than FA tier!!!

- All Storage / Month
	- $0.004 per GB

##### Archive Access Tier
- All Storage / Month	
	- $0.0036 per GB

##### Deep Archive Access Tier 
- All Storage / Month	
	- $0.00099 per GB

#### S3 Express One Zone Pricing
## Lifecycle transitions

Amazon S3 supports a waterfall model for transitioning between storage classes, as shown in the diagram below:
![[Pasted image 20240514120922.png]]
#### **Supported** lifecycle transitions
- S3 Standard to ANY other storage class
- Any storage class to the S3 Glacier or S3 Glacier Deep Archive storage classes
- S3 Standard-IA storage class to the S3 Intelligent-Tiering or S3 One Zone-IA storage classes
- The S3 Intelligent-Tiering storage class to the S3 One Zone-IA storage class
- The S3 Glacier storage class to the S3 Glacier Deep Archive storage class.

#### **Unsupported** lifecycle transitions
- ANY storage class to the Amazon S3 Standard storage class. 
- Any storage class to the Reduced Redundancy storage class. 
- Amazon S3 Intelligent-Tiering storage class to the Amazon S3 Standard-IA storage class. 
- The Amazon S3 One Zone-IA storage class to the Amazon S3 Standard-IA or Amazon S3 Intelligent-Tiering storage classes. 

#### Minimum storage duration for transitioning
- 30 days before transition from S3 Standard to S3 Standard-IA
- 30 days before transition from S3 Standard-IA One-Zone IA

## S3 Req Types
### [PUT](https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutObject.html)
### [COPY](https://docs.aws.amazon.com/AmazonS3/latest/API/API_CopyObject.html)
### [POST](https://docs.aws.amazon.com/AmazonS3/latest/API/RESTObjectPOST.html)
### [LIST](https://docs.aws.amazon.com/AmazonS3/latest/API/API_ListObjects.html)
### [GET](https://docs.aws.amazon.com/AmazonS3/latest/API/API_GetObject.html)
### [SELECT](https://docs.aws.amazon.com/AmazonS3/latest/API/API_SelectObjectContent.html)
### [DELETE]()
### [CANCEL]()
### [Livecycle Transition](https://docs.aws.amazon.com/AmazonS3/latest/userguide/lifecycle-transition-general-considerations.html)
### [Data Retrievals](https://docs.aws.amazon.com/AmazonS3/latest/userguide/restoring-objects.html)
