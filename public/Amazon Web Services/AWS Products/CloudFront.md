---
icon: AiCloudFront
aliases:
  - Amazon CloudFront
---
# Overview
- Amazon CloudFront is a fast content delivery network (CDN) service that securely delivers data, videos, applications, and APIs to customers globally with low latency, high transfer speeds, all within a developer-friendly environment.

- [[Global AWS Services|Global]] in scope

## Edge Locations (Points of Presence)
An AWS Edge location is a site that CloudFront uses to cache copies of the content for faster delivery to users at any location. 

Think read performance

There are 216 points of presence globally

![[Pasted image 20240420191428.png]]

## CloudFront Origins
- S3 bucket
	- For distributing files and caching them at the edge
	- Security
		- modding s3 bucket policy
		- Enhanced security with CloudFront **Origin Access Control (OAC)**
			- OAC is replacing Origin Access Identity (OAI) 
	- CloudFront can be used as an ingress (to upload files to S3)
- Custom Origins ([[Hypertext Transfer Protocol|HTTP]])
	-  [[Elastic Load Balancing#Application load balancer]]
	- [[Elastic Cloud Compute|EC2]] instance
	- [[Simple Storage Service|S3]] **static** website
		- bucket needs static s3 hosting enabled as it is not by default

## CloudFront vs S3 Cross Region Replication
- <mark style="background: #FF5582A6;">CloudFront</mark>
	- Global
	- Cached for TTL (~24 hours)
	- For static content that must be available everywhere
- [[Simple Storage Service#S3 Cross Region Replication|S3 CRR]]
	- Requires setup for each targetted region of replication
	- Files updated live (near real-time)
	- Read only

### Pricing
- Cost of data out per edge location VARIES
- The more out, the lower the cost becomes
- ![[Pasted image 20240423203402.png]]
### Prices Classes
- There are three price classes
	1. Price Class All: all regions -  best performance
	2. Price Class 200: most regions, but excluding most expensive regions
	3. Price Class 100: ONLY the least expensive regions
- Refer to the graphics below for visualizing these classes
- ![[Pasted image 20240423203941.png]]
- ![[Pasted image 20240423204039.png]]

#### Exam perspectives
- If you see "[[Content Delivery Network]]," you should be thinking CloudFront
- 


 