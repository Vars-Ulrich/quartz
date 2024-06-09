---
icon: AiApplicationMigrationService
aliases:
  - AWS Application Migration Service
---
# Overview

AWS Application Migration Service (AWS MGN), formerly known as CloudEndure Migration, is a service provided by Amazon Web Services designed to simplify, expedite, and reduce the cost of cloud migrations. It achieves this by offering a highly automated lift-and-shift solution that is suitable for moving applications from any physical, virtual, or cloud-based infrastructure to AWS.

### Key Features of AWS Application Migration Service

1. **Automated Lift-and-Shift**: AWS MGN automates the process of lifting your existing servers to the cloud (AWS), shifting them into a new, cloud-native environment. This includes operating systems, databases, applications, and their configurations.
    
2. **Minimal Downtime**: The service is designed to minimize downtime during the migration process. It continually replicates source servers to AWS, allowing the migration to be completed with minimal disruption to operational processes.
    
3. **Block-Level Replication**: It uses continuous block-level data replication, which ensures data consistency and significantly reduces the cutover windows during the migration.
    
4. **Support for Various Source Environments**: AWS MGN can migrate from any source environment — including physical servers, VMware, Hyper-V, and other clouds like Azure or Google Cloud Platform.
    
5. **Test Mode**: Before performing the actual migration, AWS MGN allows you to conduct test launches of your replicated servers in AWS without impacting the source servers. This helps ensure that everything works correctly in the AWS environment before going live.
    
6. **Integrated with AWS Services**: Once the servers are migrated, they can leverage various AWS services like Amazon EC2, Amazon RDS, AWS Elastic Beanstalk, and others to enhance performance, security, and reliability.
    

### How It Works

- **Setup and Configuration**: Begin by setting up the AWS MGN by defining your source servers and target AWS environment.
- **Replication**: Install a lightweight agent on your source servers, which then replicates all server data to a staging area in AWS at block level. This replication includes system disks and configurations.
- **Testing**: Conduct tests on your replicated servers in AWS to verify that everything operates as expected without affecting your live environment.
- **Cutover**: Once testing is confirmed, perform a cutover to switch traffic from the source servers to the AWS servers. This step is designed to have minimal downtime and is typically scheduled for off-peak hours.
- **Post-Migration**: After migration, decommission the source servers and start optimizing your environment in AWS to take full advantage of cloud-native features and services.

### Benefits

- **Cost Efficiency**: Reduces the cost of migration by automating many of the steps that would otherwise require significant manual effort and custom scripting.
- **Speed**: Accelerates the migration process, allowing businesses to quickly benefit from the flexibility and scalability of AWS.
- **Simplicity**: Provides a straightforward process for migrating complex, multi-tier applications without the need to modify them.
- **Risk Mitigation**: Minimizes downtime and operational impact, providing businesses with a reliable way to transition to AWS.

### Use Cases

- **Data Center Exit**: Ideal for companies looking to close their data centers and move entirely to the cloud.
- **Disaster Recovery**: Can be used to improve business continuity planning by facilitating easier and more reliable disaster recovery solutions on AWS.
- **Application Modernization**: While initially offering a lift-and-shift, AWS MGN can serve as a stepping stone to further modernization on AWS, such as refactoring applications to take advantage of AWS-native services.

AWS Application Migration Service is a robust tool for organizations seeking a low-friction path to cloud migration, providing a suite of capabilities designed to simplify the transition and reduce associated risks and costs.