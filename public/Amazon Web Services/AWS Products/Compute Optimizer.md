---
icon: AiComputeOptimizer
---
# Overview
AWS Compute Optimizer recommends optimal [[amazon web services|AWS]] resources for your workloads to reduce costs and improve performance by using machine learning to analyze historical utilization metrics. Over-provisioning resources can lead to unnecessary infrastructure costs, and under-provisioning resources can lead to poor application performance. Compute Optimizer helps you choose optimal configurations for three types of AWS resources: Amazon [[Elastic Cloud Compute|EC2]] instances, Amazon [[Elastic Block Store|EBS]] volumes, and AWS [[Lambda]] functions, based on your utilization data.
Compute Optimizer recommends up to 3 options from 140+ EC2 instance types, as well as a wide range of EBS volume and Lambda function configuration options, to right-size your workloads. Compute Optimizer also projects what the [[Central Processing Unit|CPU]] utilization, [[Computer memory|memory]] utilization, and run time of your workload would have been on recommended AWS resource options. This helps you understand how your workload would have performed on the recommended options before implementing the recommendations.

- Supports
	- [[Elastic Cloud Compute|EC2]] instances
	- [[EC2 Auto-Scaling]] groups
	- [[Elastic Block Store|EBS]] volumes
	- [[Lambda]] functions

- Lower costs
	- up to 25%


Recommendations can be exported to s3

AWS Compute Optimizer helps you identify the optimal AWS resource configurations, such as Amazon EC2 instance types, Amazon EBS volume configurations, and AWS Lambda function memory sizes, using machine learning to analyze historical utilization metrics. AWS Compute Optimizer delivers recommendations for selected types of EC2 instances, EC2 Auto Scaling groups, EBS volumes, and Lambda functions.

Compute Optimizer calculates an individual performance risk score for each resource dimension of the recommended instance, including CPU, memory, EBS throughput, EBS IOPS, disk throughput, disk throughput, network throughput, and network packets per second (PPS).

AWS Compute Optimizer provides EC2 instance type and size recommendations for [[EC2 Auto-Scaling|EC2 Auto Scaling]] groups with a fixed group size, meaning desired, minimum, and maximum are all set to the same value and have no scaling policy attached.

AWS Compute Optimizer supports IOPS and throughput recommendations for General Purpose (SSD) (gp3) volumes and IOPS recommendations for Provisioned IOPS (io1 and io2) volumes.

Compute Optimizer helps you optimize two categories of Lambda functions. The first category includes Lambda functions that may be over-provisioned in memory sizes. The second category includes compute-intensive Lambda functions that may benefit from additional CPU power.