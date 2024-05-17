---
sticker: vault//Media/icons/aws-icons/ServerMigrationService.svg
---
# Overview

### Service Overview:

AWS Server Migration Service (SMS) is an agentless service that helps you migrate on-premises virtual machines (VMs), VMware VMs, and [[Microsoft Hyper-V]] VMs to AWS quickly, securely, and with minimal downtime. It simplifies the migration process by automating the bulk of the migration tasks, including server discovery, replication, and cutover, while providing real-time progress tracking and validation to ensure a successful migration.

### Key Features:

1. **Agentless Migration**: SMS performs migration tasks without requiring agents to be installed on source servers, minimizing the impact on source workloads and simplifying the migration process.
2. **Server Discovery**: SMS automatically discovers on-premises servers, VMware VMs, and Hyper-V VMs in your environment, allowing you to select servers for migration from a centralized console.
3. **Incremental Replication**: SMS replicates server data to AWS in incremental, block-level updates, minimizing the amount of data transferred and reducing migration time and bandwidth requirements.
4. **Real-time Progress Tracking**: SMS provides real-time progress tracking and status updates during migration, allowing you to monitor the status of each server migration and troubleshoot any issues as they arise.
5. **Validation and Testing**: SMS includes pre-migration testing capabilities to validate server compatibility and readiness for migration, ensuring a successful migration with minimal downtime and risk.
6. **Continuous Data Replication**: SMS supports continuous data replication, allowing you to keep source and target servers synchronized during the migration process and minimize data loss in the event of cutover.
7. **Automated Cutover**: SMS automates the cutover process, allowing you to switch over to AWS target servers seamlessly and with minimal disruption to business operations.
8. **Integration with AWS Services**: SMS integrates with other AWS services, such as AWS CloudEndure Migration, AWS Migration Hub, and AWS Database Migration Service (DMS), to provide a comprehensive migration solution for heterogeneous environments.
9. **Security and Compliance**: SMS ensures data security and compliance during migration by encrypting data in transit and at rest, adhering to AWS security best practices, and providing audit logs and compliance reports.

### How It Works:

1. **Setup**: You set up the SMS service in the AWS Management Console and configure the replication server endpoint, IAM roles, and network settings to establish connectivity between your on-premises environment and AWS.
2. **Server Discovery**: SMS automatically discovers on-premises servers, VMware VMs, and Hyper-V VMs in your environment and provides a list of servers eligible for migration.
3. **Replication**: You select the servers to migrate and configure replication settings, including replication frequency, target AWS Region, and encryption options. SMS initiates replication and begins transferring server data to AWS.
4. **Validation and Testing**: SMS performs pre-migration testing to validate server compatibility and readiness for migration, identifying any issues that may impact the migration process.
5. **Continuous Replication**: SMS supports continuous data replication, keeping source and target servers synchronized during the migration process to minimize data loss and ensure consistency.
6. **Cutover**: Once replication is complete and servers are validated, you initiate the cutover process to switch over to AWS target servers. SMS automates the cutover process, minimizing downtime and disruption to business operations.
7. **Post-migration Cleanup**: After migration is complete, SMS performs post-migration cleanup tasks, including decommissioning source servers and updating DNS records, to finalize the migration process.

### Benefits:

1. **Simplified Migration**: SMS simplifies the migration process by automating server discovery, replication, and cutover tasks, reducing the complexity and risk associated with migrating on-premises servers to AWS.
2. **Minimal Downtime**: SMS minimizes downtime during migration by performing continuous data replication and automating the cutover process, allowing you to migrate workloads with minimal disruption to business operations.
3. **Real-time Monitoring**: SMS provides real-time progress tracking and status updates during migration, allowing you to monitor the status of each server migration and troubleshoot any issues as they arise.
4. **Cost-effective**: SMS helps reduce migration costs by optimizing data transfer and minimizing downtime, allowing you to migrate workloads efficiently and cost-effectively.
5. **Security and Compliance**: SMS ensures data security and compliance during migration by encrypting data in transit and at rest, adhering to AWS security best practices, and providing audit logs and compliance reports.
6. **Scalability**: SMS is designed to scale with your migration needs, allowing you to migrate single servers or entire data centers to AWS quickly and efficiently.
7. **Integration with AWS Services**: SMS integrates with other AWS services, such as AWS CloudEndure Migration, AWS Migration Hub, and AWS Database Migration Service (DMS), to provide a comprehensive migration solution for heterogeneous environments.

### Use Cases:

1. **Data Center Migration**: Use SMS to migrate on-premises data centers to AWS, consolidating infrastructure, reducing costs, and leveraging cloud scalability and agility.
2. **VMware to AWS Migration**: Use SMS to migrate VMware virtualized workloads to AWS, leveraging existing VMware investments while benefiting from AWS cloud services and capabilities.
3. **Hyper-V to AWS Migration**: Use SMS to migrate Microsoft Hyper-V virtualized workloads to AWS, modernizing infrastructure and accelerating digital transformation initiatives.
4. **Disaster Recovery**: Use SMS to implement disaster recovery solutions by replicating on-premises workloads to AWS, ensuring business continuity and data protection in the event of a disaster.
5. **Cloud Migration Projects**: Use SMS as part of cloud migration projects to migrate workloads to AWS quickly, securely, and with minimal downtime, accelerating time-to-value and reducing risk.

AWS Server Migration Service (SMS) provides a comprehensive solution for migrating on-premises servers, VMware VMs, and Microsoft Hyper-V VMs to AWS quickly, securely, and with minimal downtime, enabling organizations to modernize infrastructure and accelerate their cloud migration journey.