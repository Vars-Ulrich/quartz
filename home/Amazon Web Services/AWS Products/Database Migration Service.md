---
sticker: vault//Media/icons/aws-icons/DatabaseMigrationService.svg
aliases:
  - DMS
---
# Overview
AWS Database Migration Service helps you migrate databases to AWS quickly and securely. The source database remains fully operational during the migration, minimizing downtime to applications that rely on the database. The AWS Database Migration Service can migrate your data to and from the most widely used commercial and open-source databases.

### Service Overview:

AWS Database Migration Service (DMS) is a fully managed service that helps users migrate databases to AWS quickly, securely, and seamlessly. It supports homogeneous migrations (e.g., Oracle to Oracle) as well as heterogeneous migrations (e.g., Oracle to Amazon Aurora), enabling users to move data between different database platforms with minimal downtime and disruption.

### Key Features:

1. **Homogeneous and Heterogeneous Migration**: DMS supports both homogeneous and heterogeneous migrations, allowing users to migrate data between databases of the same or different platforms, such as Oracle, SQL Server, MySQL, PostgreSQL, MongoDB, and Amazon Aurora.
2. **Continuous Data Replication**: DMS enables continuous data replication from the source database to the target database, ensuring data consistency and minimizing downtime during the migration process.
3. **Schema Conversion**: DMS can automatically convert the schema of the source database to match the target database, facilitating seamless migration between different database engines.
4. **Full Load and CDC**: DMS supports full load and change data capture (CDC) migration methods, allowing users to migrate existing data and capture ongoing changes in real-time.
5. **Data Validation**: DMS provides built-in data validation capabilities to ensure data integrity and accuracy before, during, and after the migration process.
6. **Flexible Replication Instance Options**: DMS offers a range of replication instance types and configurations to meet different migration requirements, providing scalability, performance, and cost-effectiveness.
7. **Security and Compliance**: DMS ensures data security and compliance during migrations by encrypting data in transit and at rest, supporting SSL connections, and integrating with AWS Identity and Access Management (IAM) for access control.
8. **Monitoring and Logging**: DMS provides monitoring metrics and logging capabilities to track the progress of migrations, monitor replication latency, and troubleshoot issues.
9. **High Availability**: DMS supports high availability configurations with multi-AZ replication instances and automatic failover, ensuring continuous data replication and minimal downtime.
10. **Integration with AWS Services**: DMS integrates with other AWS services such as AWS Schema Conversion Tool (SCT), AWS Database Query Tool (DQT), AWS CloudFormation, and AWS Management Console, enabling seamless migration workflows and automation.

### How It Works:

1. **Source and Target Database Configuration**: Users configure the source and target databases in the DMS console, specifying connection details, credentials, and migration settings.
2. **Replication Instance Provisioning**: Users provision a replication instance in the desired AWS region, selecting the instance type, size, and configuration to meet migration requirements.
3. **Migration Task Creation**: Users create a migration task in the DMS console, specifying the source and target database endpoints, replication settings, and migration method (e.g., full load, CDC).
4. **Data Replication**: DMS starts replicating data from the source database to the target database according to the migration task settings, continuously synchronizing data changes in real-time.
5. **Schema Conversion (Optional)**: If schema conversion is required, DMS automatically converts the schema of the source database objects to match the target database, applying data type mappings and compatibility rules.
6. **Data Validation and Cutover**: DMS performs data validation checks to ensure data integrity and accuracy, allowing users to verify the migration results before performing the cutover to the target database.
7. **Cutover and Post-migration Tasks**: Once validation is complete, users perform the cutover to switch production traffic to the target database. DMS provides post-migration tasks to clean up resources and finalize the migration process.

### Benefits:

1. **Minimized Downtime**: DMS enables live migrations with minimal downtime, allowing users to migrate databases with no or minimal impact on application availability.
2. **Simplified Migration Process**: DMS automates and streamlines the migration process, reducing manual effort and complexity associated with database migrations.
3. **Reduced Risk**: DMS provides built-in data validation and monitoring capabilities, helping users mitigate risks and ensure data integrity throughout the migration process.
4. **Scalability and Flexibility**: DMS supports migrations of any size and complexity, with flexible replication instance options and configuration settings to meet diverse migration requirements.
5. **Cost-effectiveness**: DMS offers a pay-as-you-go pricing model with no upfront fees or long-term commitments, allowing users to pay only for the resources and migrations they use.
6. **Integration with AWS Ecosystem**: DMS integrates seamlessly with other AWS services, enabling users to leverage AWS tools and services for end-to-end migration workflows and automation.

### Use Cases:

1. **Database Consolidation**: Organizations use DMS to consolidate multiple databases into a single database platform, simplifying management and reducing infrastructure costs.
2. **Database Migration to AWS**: DMS helps organizations migrate on-premises databases to AWS, enabling them to take advantage of the scalability, reliability, and cost-effectiveness of cloud computing.
3. **Database Replication and Disaster Recovery**: DMS facilitates database replication and disaster recovery strategies by continuously replicating data to standby databases or secondary AWS regions.
4. **Database Platform Migration**: DMS enables organizations to migrate databases between different database platforms, such as Oracle to Amazon Aurora, SQL Server to MySQL, or MongoDB to Amazon DocumentDB.
5. **Data Center Exit Strategy**: Organizations use DMS as part of their data center exit strategy to migrate databases from on-premises data centers to the cloud, reducing data center footprint and operational overhead.

AWS Database Migration Service simplifies and accelerates database migrations to AWS, enabling organizations to migrate databases with confidence, minimize downtime, and unlock the benefits of cloud computing.
