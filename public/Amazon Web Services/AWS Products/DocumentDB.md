---
icon: AiDocumentDB
aliases:
  - Amazon DocumentDB
---
# Overview

AWS DocumentDB (with MongoDB compatibility) is a fully managed NoSQL database service provided by Amazon Web Services that supports MongoDB workloads. As a document-oriented database, AWS DocumentDB is designed to store, retrieve, and manage semi-structured data. The service aims to make it simple and cost-effective to operate large scale MongoDB workloads in the cloud with compatibility for MongoDB applications and tools.

- Whereas Aurora is an AWS implementation of PostgreSQL / MySQL, DocumentDB is the same for [[MongoDB]] **NoSQL database** 
- MongoDB
	- used to store, query, and index JSON data
- Similar deployment concepts as [[Aurora]]
- Fully Managed
- Highly available 
	- replication across 3 AZ
- Document DB automatically grows in increments of 10GB
- Automatically scales to workloads with **millions of reqs/sec**
- 

### Key Features of AWS DocumentDB

1. **MongoDB Compatibility**: AWS DocumentDB is compatible with MongoDB, meaning it supports the same MongoDB application code, drivers, and tools. Developers can use it as a drop-in replacement for MongoDB without needing to rewrite their application logic.
    
2. **Fully Managed**: As a managed service, AWS DocumentDB handles time-consuming maintenance tasks such as hardware provisioning, patching, setup, configuration, and backups.
    
3. **Scalability**: It offers the ability to scale the compute and memory resources associated with an instance up or down with minimal downtime, and also allows scaling the storage automatically as data grows.
    
4. **High Availability and Durability**: AWS DocumentDB is designed for fault tolerance and high availability. It automatically replicates six copies of your data across three AWS Availability Zones and continuously backs up your data to Amazon S3. It supports point-in-time recovery, helping you safeguard and recover your data.
    
5. **Performance Monitoring**: Integrates with Amazon CloudWatch to provide detailed monitoring and alerting for metrics such as compute utilization, storage, and throughput, helping you optimize performance.
    
6. **Security**: Offers built-in security features such as encryption at rest using AWS Key Management Service (KMS) and encryption in transit with TLS. AWS Identity and Access Management (IAM) can be used to control access to DocumentDB resources.
    

### How It Works

- **Setup**: You can launch an AWS DocumentDB cluster from the AWS Management Console, specifying your desired instance size, number of instances, and replication settings.
    
- **Database Operations**: Once set up, you can connect to your database using MongoDB compatible drivers. You can perform CRUD (Create, Read, Update, Delete) operations and other database operations just as you would with a MongoDB database.
    
- **Scaling and Management**: Adjust the scale of your database cluster through the AWS Management Console, adding or removing instances as needed. Monitor performance and set up alerts in Amazon CloudWatch.
    
- **Backup and Recovery**: AWS DocumentDB automatically backs up your data continuously to Amazon S3, and retains backups for a user-defined period to support point-in-time recovery.
    

### Benefits

- **Ease of Migration**: Since it is compatible with MongoDB, migrating existing MongoDB databases to AWS DocumentDB can be straightforward, often requiring no changes to application code.
    
- **Reduced Management Overhead**: Being a fully managed service, it reduces the operational burden on your team, allowing them to focus on development rather than on database management and maintenance.
    
- **Cost-Effective**: You pay only for the resources you provision, and there is no need for upfront investments, making it cost-effective for varying workloads.
    

### Use Cases

- **Web and Mobile Applications**: Commonly used for backend services for web and mobile applications, particularly when handling varied and changing data formats.
    
- **Content Management**: Suitable for content management systems (CMS) where documents and their metadata need to be stored and managed efficiently.
    
- **Catalogs and User Profiles**: Often used for storing user profiles and product catalogs in e-commerce and digital media applications, due to its flexible schema and scalability.
    

AWS DocumentDB provides a powerful, scalable, and fully managed document database solution that aligns well with the needs of modern application development that requires flexible schema and efficient data management.