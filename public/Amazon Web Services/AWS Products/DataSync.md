---
icon: AiDataSync
---
# Overview
- AWS DataSync is a secure online data transfer service that simplifies, automates, and accelerates copying terabytes of data to and from AWS storage services. Easily migrate or replicate large data sets without having to build custom solutions or oversee repetitive tasks. DataSync can copy data between [[Network File System|Network File System (NFS)]] shares, or [[Server Message Block|Server Message Block (SMB)]] shares, self-managed object storage, [[Snowcone|AWS Snowcone]], [[Simple Storage Service|Amazon Simple Storage Service (Amazon S3)]] buckets, [[Elastic File System (EFS)|Amazon Elastic File System (Amazon EFS)]] file systems, and [[FSx|Amazon FSx]] for Windows File Server file systems.

	- You can use AWS DataSync for ongoing transfers from on-premises systems into or out of AWS for processing. DataSync can help speed up your critical hybrid cloud storage workflows in industries that need to move active files into AWS quickly. This includes machine learning in life sciences, video production in media and entertainment, and big data analytics in financial services. DataSync provides timely delivery to ensure dependent processes are not delayed. You can specify exclude filters, include filters, or both, to determine which files, folders or objects get transferred each time your task runs.

- AWS DataSync employs an AWS-designed transfer protocol—decoupled from the storage protocol—to accelerate data movement. The protocol performs optimizations on how, when, and what data is sent over the network. Network optimizations performed by DataSync include incremental transfers, in-line compression, and sparse file detection, as well as in-line data validation and encryption.

### Service Overview:

AWS DataSync is a fully managed data transfer service that simplifies and accelerates moving data between on-premises storage systems and AWS services. It enables organizations to transfer large amounts of data quickly, securely, and cost-effectively, whether for migration, replication, or data processing purposes.

### Key Features:

1. **High-speed Data Transfer**: DataSync uses a purpose-built data transfer protocol optimized for high-speed data transfer, maximizing network bandwidth and minimizing transfer times.
2. **Incremental Data Transfer**: DataSync supports incremental data transfers, only transferring the changes (delta) since the last synchronization, reducing the time and resources required for subsequent transfers.
3. **Automatic Encryption**: DataSync encrypts data in transit using TLS encryption, ensuring data security and confidentiality during transfer between on-premises storage and AWS services.
4. **Data Integrity Checking**: DataSync performs data integrity checks during transfer to ensure that data arrives intact and uncorrupted at the destination, providing assurance of data reliability and consistency.
5. **Bandwidth Throttling and Scheduling**: DataSync allows users to control the bandwidth utilization during data transfer, enabling them to throttle the transfer rate and schedule transfers to minimize network congestion and impact on production workloads.
6. **Support for Multiple Protocols**: DataSync supports various protocols for accessing on-premises storage, including Network File System (NFS), Server Message Block (SMB), and Amazon S3-compatible object storage, providing flexibility and compatibility with different storage systems.
7. **Integration with AWS Services**: DataSync seamlessly integrates with other AWS services such as Amazon S3, Amazon EFS, Amazon FSx for Windows File Server, and Amazon FSx for Lustre, enabling users to transfer data to and from these services with ease.
8. **On-premises Data Agents**: DataSync deploys lightweight agents on-premises to facilitate data transfer between on-premises storage systems and AWS, providing a secure and efficient data transfer mechanism.
9. **Data Transfer Optimization**: DataSync automatically optimizes data transfer performance based on network conditions and available resources, ensuring efficient and reliable data transfer even over high-latency or low-bandwidth networks.
10. **Monitoring and Logging**: DataSync provides monitoring metrics and logging capabilities to track the progress of data transfers, monitor transfer performance, and troubleshoot issues, enabling users to ensure data transfer success and reliability.

### How It Works:

1. **Agent Deployment**: Users deploy DataSync agents on-premises within their data center or environment, configuring them to connect to the on-premises storage systems.
2. **Task Creation**: Users create data transfer tasks in the AWS Management Console or through the AWS CLI/API, specifying the source and destination locations, transfer settings, and scheduling options.
3. **Data Transfer**: DataSync agents initiate data transfer tasks, retrieving data from the source storage, encrypting it in transit, and transferring it securely to the destination storage in AWS.
4. **Incremental Sync**: For subsequent data transfer tasks, DataSync agents perform incremental syncs, transferring only the changes or updates since the last synchronization, minimizing transfer times and network bandwidth usage.
5. **Data Integrity Checks**: DataSync verifies the integrity of transferred data using checksums or hash functions, ensuring data consistency and reliability at the destination.
6. **Monitoring and Logging**: Users monitor the progress of data transfer tasks using the AWS Management Console or CloudWatch metrics, accessing logs and status updates to track transfer performance and troubleshoot any issues that may arise.

### Benefits:

1. **Fast and Efficient Data Transfer**: DataSync enables high-speed data transfer between on-premises storage and AWS services, maximizing network bandwidth and minimizing transfer times.
2. **Data Security and Encryption**: DataSync encrypts data in transit using TLS encryption, ensuring data security and confidentiality during transfer, with optional encryption at rest in AWS storage services.
3. **Incremental Data Transfer**: DataSync supports incremental data transfers, transferring only the changes since the last synchronization, reducing transfer times and network bandwidth usage for subsequent transfers.
4. **Flexible Integration**: DataSync seamlessly integrates with various AWS storage services, enabling users to transfer data to and from Amazon S3, Amazon EFS, and Amazon FSx with ease.
5. **Simplified Management**: DataSync is fully managed by AWS, eliminating the need for manual management of data transfer infrastructure and simplifying data migration and replication workflows.
6. **Scalability and Reliability**: DataSync scales automatically to handle large data volumes and accommodates fluctuating workloads, ensuring reliable and consistent data transfer performance.
7. **Cost-effectiveness**: DataSync offers a pay-as-you-go pricing model with no upfront fees or long-term commitments, allowing users to pay only for the data transfer resources and usage they consume.

### Use Cases:

1. **Data Migration to AWS**: Organizations use DataSync to migrate large datasets from on-premises storage systems to AWS services such as Amazon S3, Amazon EFS, or Amazon FSx, enabling them to take advantage of cloud storage scalability, durability, and cost-effectiveness.
2. **Data Replication and Backup**: DataSync facilitates data replication and backup strategies by continuously synchronizing data between on-premises storage and AWS, providing disaster recovery, data protection, and business continuity capabilities.
3. **Data Processing and Analytics**: DataSync enables organizations to transfer data to AWS for processing and analytics purposes, supporting use cases such as data warehousing, big data analytics, machine learning, and IoT data ingestion.
4. **Hybrid Cloud Storage**: Organizations with hybrid cloud environments use DataSync to bridge on-premises storage with AWS cloud storage, enabling seamless data transfer and access across distributed environments while maintaining data consistency and integrity.

AWS DataSync simplifies and accelerates data transfer to AWS, enabling organizations to migrate, replicate, and process data quickly, securely, and cost-effectively, unlocking the benefits of cloud computing for their data-intensive workloads.
