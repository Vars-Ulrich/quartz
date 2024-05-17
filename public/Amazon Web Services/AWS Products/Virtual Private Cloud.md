---
sticker: vault//Media/icons/aws-icons/VirtualPrivateCloud.svg
aliases:
  - VPC
---
# Virtual Private Cloud
- Amazon Virtual Private Cloud (Amazon VPC) is a logically isolated section of the AWS Cloud where you can launch AWS resources in a virtual network that you define. You have complete control over your virtual networking environment, including the selection of your IP address range, creation of subnets, and configuration of route tables and network gateways. 
- A VPC spans all of the Availability Zones in the Region.
- A subnet is a range of IP addresses within your VPC. A subnet spans only one Availability Zone in the Region.

## Internet Gateway (IGW)
- Connects resources in a VPC to the internet
- scales horizontally
- highly available
- redundant
- 

## VPC endpoint gateway



- only used with:
	- [[Simple Storage Service|S3]]
	- [[DynamoDB]]
- ALL other services that support VPC Endpoints use a VPC Endpoint Interface

## VPC endpoint interface

An interface VPC endpoint (interface endpoint) enables you to connect to services powered by AWS PrivateLink. It is **not** a component of a connection between on-premises network and AWS.

## VPC Peering
Is not transitive and is, therefore, Difficult to manage

![[SAA Course Slides.pdf#page=686|SAA Course Slides, VPC]]

[[SAA Course Slides.pdf#page=688&selection=14,0,17,0|SAA Course Slides, page 688]]

#### Exam Alerts
##### [[IPv6]] Troubleshooting
- [[IPv4]] CANNOT be disabled for you VPC and subnets
- So if you can't launch an EC2 instance in your subnet
	- It is not because you cannot acquire an IPv6 instance in your subnet
	- Rather, it is because there are no available IPv4 in your subnet
- Solution: create a new IPv4 CIDR in your subnet
