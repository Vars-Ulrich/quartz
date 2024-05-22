---
icon: AiS3OnOutposts
---
# Overview

### Service Overview:

Amazon S3 on Outposts brings the benefits of Amazon Simple Storage Service (S3) to on-premises environments by extending the S3 storage infrastructure to AWS Outposts. It allows customers to store and manage data locally on Outposts while still benefiting from the scalability, durability, and reliability of S3.

### Key Features:

1. **Local Data Storage**: S3 on Outposts allows you to store and manage data locally on AWS Outposts, providing low-latency access to data for applications running in on-premises environments.
2. **S3 API Compatibility**: The service is fully compatible with the S3 API, allowing you to use existing S3 applications, tools, and workflows seamlessly with S3 on Outposts.
3. **Durability and Reliability**: S3 on Outposts provides the same durability and reliability guarantees as standard S3 storage, with data replicated across multiple devices within the Outposts environment.
4. **Data Transfer Options**: You can transfer data between S3 on Outposts and other S3 storage classes (e.g., S3 in the AWS Region) using AWS DataSync, AWS Direct Connect, or other data transfer methods.
5. **Integration with AWS Services**: S3 on Outposts seamlessly integrates with other AWS services such as AWS Lambda, Amazon EC2, and Amazon EBS, enabling you to build hybrid applications that span on-premises and cloud environments.
6. **Local Data Processing**: You can perform data processing and analytics locally on Outposts using services like Amazon EMR, Amazon Redshift, or custom applications running on Amazon EC2 instances.

### How It Works:

1. **Deployment**: AWS deploys Outposts to your on-premises location, extending the AWS infrastructure to your data center, co-location space, or edge location.
2. **Configuration**: You configure S3 on Outposts using the AWS Management Console, AWS CLI, or AWS SDKs, specifying storage capacity, access policies, and replication options.
3. **Data Storage**: You store data locally on S3 on Outposts using the same S3 API and tools you use with standard S3 storage.
4. **Data Management**: You can manage data stored in S3 on Outposts, including uploading, downloading, and deleting objects, using standard S3 management capabilities.
5. **Data Replication**: S3 on Outposts replicates data across multiple devices within the Outposts environment, providing durability and reliability similar to standard S3 storage.
6. **Integration**: You can integrate S3 on Outposts with other AWS services and applications running on Outposts or in the AWS cloud, enabling hybrid cloud architectures and data workflows.

### Benefits:

1. **Hybrid Cloud Storage**: S3 on Outposts enables hybrid cloud storage solutions, allowing you to store data locally on-premises while still leveraging the benefits of AWS cloud services.
2. **Low-Latency Data Access**: By storing data locally on Outposts, you can achieve low-latency access to data for applications running in on-premises environments, improving performance and responsiveness.
3. **S3 Compatibility**: S3 on Outposts is fully compatible with the S3 API, ensuring seamless integration with existing S3 applications, tools, and workflows.
4. **Data Consistency**: Data stored in S3 on Outposts is consistent with data stored in standard S3 storage classes, ensuring consistency and interoperability across hybrid cloud environments.
5. **Scalability**: S3 on Outposts scales seamlessly to accommodate growing storage requirements, allowing you to scale up or down based on demand without provisioning additional infrastructure.
6. **Data Sovereignty**: S3 on Outposts provides control over data residency and sovereignty, allowing you to store sensitive or regulated data locally on-premises while still benefiting from AWS services and capabilities.

### Use Cases:

1. **Data Residency Requirements**: Store sensitive or regulated data locally on-premises to meet data residency and compliance requirements while still leveraging AWS services and capabilities.
2. **Low-Latency Applications**: Deploy applications with low-latency data access requirements in on-premises environments using S3 on Outposts to store and manage data locally.
3. **Edge Computing**: Support edge computing applications and use cases by storing data locally on Outposts at the edge, enabling real-time data processing and analysis.
4. **Disconnected Environments**: Deploy AWS services and applications in disconnected or intermittently connected environments using Outposts with S3 for local data storage and processing.
5. **Data Migration**: Use S3 on Outposts as a staging area for data migration or replication between on-premises environments and the AWS cloud, minimizing data transfer costs and latency.

Amazon S3 on Outposts brings the power of AWS cloud storage to on-premises environments, enabling hybrid cloud storage solutions, low-latency data access, and seamless integration with AWS services and applications. With S3 on Outposts, you can store and manage data locally while still benefiting from the scalability, durability, and reliability of Amazon S3.