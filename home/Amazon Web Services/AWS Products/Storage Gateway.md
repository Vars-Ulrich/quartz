---
sticker: vault//Media/icons/aws-icons/StorageGateway.svg
---
# Storage Gateway
AWS Storage Gateway is a hybrid cloud storage service that connects your existing on-premises environments with the AWS Cloud. Customers use Storage Gateway to simplify storage management and reduce costs for key hybrid cloud storage use cases.
Encryption enabled automatically

AWS Storage Gateway is a hybrid cloud storage service that connects your existing onpremises environments with the AWS Cloud. Customers use Storage Gateway to simplify storage management and reduce costs for key hybrid cloud storage use cases. These include moving tape backups to the cloud, reducing on-premises storage with cloud-backed file shares, providing low latency access to data in AWS for on-premises applications, as well as various migration, archiving, processing, and disaster recovery use cases.

AWS Storage Gateway service provides three different types of gateways – Tape Gateway, File Gateway, and Volume Gateway – that seamlessly connect on-premises applications to cloud storage, caching data locally for low-latency access.

### Tape Gateway:
function


### File Gateway
- you can choose from two file gateway types for your latency-sensitive applications and workloads that require local caching and file protocol access.
	- Amazon S3 File Gateway
	- Amazon FSx File Gateway

function: provides access to objects in S3 as files or file share mount points.

- With a file gateway, you can do the following 
	- store and retrieve files directly using the NFS version 3 or 4.1 protocol.
	- store and retrieve files directly using the SMB file system version, 2 and 3 protocol.
	- access your data directly in Amazon S3 from any AWS Cloud application or service.
	- manage your Amazon S3 data using lifecycle policies, cross-region replication, and versioning. You can think of a file gateway as a file system mount on S3.


### Volume Gateway
function


https://docs.aws.amazon.com/storagegateway/latest/userguide/StorageGatewayConcepts.html

https://tutorialsdojo.com/amazon-s3/
