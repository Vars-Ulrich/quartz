---
sticker: vault//Media/icons/aws-icons/FSx.svg
---
# Overview

### Service Overview:

Amazon FSx is a fully managed file storage service that makes it easy to launch and run feature-rich file systems in the AWS cloud. It provides scalable, highly available file systems compatible with popular protocols, allowing customers to access and share data across multiple compute instances and applications.

### Key Features:

1. **Fully Managed Service**: Amazon FSx is a fully managed service, eliminating the operational overhead of managing file storage infrastructure, including hardware provisioning, software updates, and backups.
2. **Compatibility**: FSx supports industry-standard file system protocols such as Network File System (NFS) and Server Message Block (SMB), making it compatible with a wide range of operating systems, applications, and workflows.
3. **High Performance**: FSx provides high-performance file systems with low latency and high throughput, optimized for a variety of workloads, including database storage, analytics, media processing, and content management.
4. **Scalability**: FSx file systems can scale seamlessly to petabyte-scale storage capacity, enabling customers to store and access large volumes of data for growing workloads and applications.
5. **Data Durability**: FSx replicates data across multiple Availability Zones (AZs) within an AWS Region to ensure data durability and availability in the event of hardware failures or AZ outages.
6. **Data Transfer**: FSx supports high-speed data transfer options, including Direct Connect and AWS DataSync, for efficient data migration, backup, and synchronization between on-premises environments and AWS cloud storage.
7. **Integration with AWS Services**: FSx integrates seamlessly with other AWS services such as Amazon EC2, AWS Lambda, AWS IAM, AWS CloudWatch, and AWS CloudTrail, enabling customers to leverage existing AWS workflows and services.
8. **Security and Compliance**: FSx provides built-in encryption at rest and in transit using AWS Key Management Service (KMS), access control using AWS IAM policies, and compliance with industry standards such as HIPAA and PCI DSS.
9. **Backup and Restore**: FSx offers automated backup and restore capabilities, allowing customers to create and retain backups of file systems at configurable intervals and restore them in case of data loss or corruption.
10. **Cost-Effective Pricing**: FSx follows a pay-as-you-go pricing model, with customers paying only for the storage capacity and throughput provisioned, making it cost-effective for both small-scale and large-scale deployments.

### How It Works:

1. **File System Creation**: Customers can create FSx file systems using the AWS Management Console, AWS CLI, or AWS SDKs, specifying the file system type (NFS or SMB), storage capacity, performance requirements, and access permissions.
2. **File System Provisioning**: FSx provisions the requested file system in the specified AWS Region, automatically configuring the underlying storage infrastructure, network connectivity, and security settings.
3. **Mounting File Systems**: Customers can mount FSx file systems on Amazon EC2 instances or on-premises servers using standard file system mounting commands or tools, such as NFS client or SMB client.
4. **Access Control**: Customers can configure access control settings for FSx file systems using AWS IAM policies, controlling who can access, read, write, and delete files within the file system.
5. **Data Transfer**: Customers can transfer data to and from FSx file systems using high-speed data transfer options such as AWS Direct Connect, AWS DataSync, or traditional file transfer protocols over the internet.
6. **Backup and Restore**: Customers can enable automated backups for FSx file systems, specifying backup retention policies and scheduling, and restore file systems from backups using the AWS Management Console or APIs.
7. **Monitoring and Management**: Customers can monitor and manage FSx file systems using AWS CloudWatch metrics, logs, and alarms, tracking performance metrics such as throughput, IOPS, and latency, and receiving notifications for system events.
8. **Scaling and Optimization**: Customers can scale FSx file systems vertically by increasing storage capacity and throughput or horizontally by adding additional file systems, optimizing performance and cost according to workload demands.

### Benefits:

1. **Simplified File Storage**: Amazon FSx simplifies file storage deployment and management, allowing customers to launch and run feature-rich file systems in minutes without the need for manual provisioning or maintenance.
2. **Compatibility and Interoperability**: FSx provides compatibility with popular file system protocols and operating systems, enabling seamless integration with existing applications, workflows, and environments.
3. **High Performance and Scalability**: FSx offers high-performance file systems with low latency and high throughput, capable of scaling to petabyte-scale storage capacity to meet the demands of growing workloads and applications.
4. **Data Durability and Availability**: FSx ensures data durability and availability by replicating data across multiple AZs within an AWS Region, providing resilience against hardware failures and AZ outages.
5. **Cost-Effective Pricing**: FSx follows a pay-as-you-go pricing model, allowing customers to pay only for the storage capacity and throughput provisioned, minimizing costs for both small-scale and large-scale deployments.
6. **Security and Compliance**: FSx provides built-in encryption, access control, and compliance features, ensuring data security and regulatory compliance for sensitive workloads and industries.
7. **Integration with AWS Services**: FSx integrates seamlessly with other AWS services, enabling customers to leverage existing AWS workflows, services, and tools for data storage, processing, analytics, and management.

### Use Cases:

1. **Enterprise Applications**: FSx is suitable for hosting enterprise applications such as Microsoft SharePoint, Microsoft Dynamics, and SAP applications that require shared file storage with Windows compatibility and high availability.
2. **Analytics and Big Data**: FSx is used for storing and processing large volumes of data for analytics and big data workloads, providing scalable file storage for Hadoop, Spark, Presto, and other analytics frameworks.
3. **Database Storage**: FSx is used for hosting databases such as Oracle, SQL Server, MySQL, and PostgreSQL, providing scalable and durable file storage for database files, logs, and backups with high performance and availability.
4. **Content Management**: FSx is used for storing and serving multimedia content, web assets, and digital media files for content management systems (CMS), digital publishing platforms, and media production workflows.
5. **Development and Testing**: FSx is used for hosting development and testing environments, providing shared file storage for source code repositories, build artifacts, and development tools with high performance and reliability.
6. **Backup and Archive**: FSx is used for storing backup copies of data, archives, and long-term retention data, providing durable and cost-effective file storage for backup applications, disaster recovery, and compliance purposes.

Amazon FSx offers customers a scalable, highly available, and feature-rich file storage solution in the AWS cloud, enabling them to store, access, and share data across distributed applications and workloads with ease and efficiency.


## FSx File Gateway
- 