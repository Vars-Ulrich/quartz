---
icon: AiDirectoryService
---
# Overview

AWS Directory Service offers multiple directory choices for customers who want to use Microsoft Active Directory (AD) or Lightweight Directory Access Protocol (LDAP) compatible directories in the AWS Cloud. This service simplifies the setup, scaling, and maintenance of directory services and is integral for managing user access to various AWS services and resources securely.

### Key Features of AWS Directory Service

1. **Microsoft AD**: AWS Directory Service for Microsoft Active Directory, also known as AWS Managed Microsoft AD, is built on actual Microsoft Active Directory and fully compatible with Windows-based applications and services. It supports features like Group Policy, trusts, and replication across AWS and on-premises Microsoft Active Directory domains.
    
2. **AD Connector**: AD Connector is designed to proxy directory requests to your on-premises Microsoft Active Directory without caching or syncing users’ data to the cloud. It's used primarily to provide single sign-on (SSO) to AWS services and applications running in AWS.
    
3. **Simple AD**: Simple AD is a cost-effective Active Directory-compatible service that is powered by Samba. It's suitable for smaller organizations with basic AD requirements but does not require Microsoft Active Directory's full feature set.
    
4. **Amazon Cognito**: While not part of AWS Directory Service directly, Amazon Cognito can integrate with AWS Directory Service to provide user sign-up, sign-in, and access control to mobile and web applications.
    
5. **Seamless Integration**: AWS Directory Service integrates with Amazon RDS for SQL Server, AWS WorkSpaces (VDI), AWS WorkDocs, and AWS WorkMail, providing directory services that are managed, scalable, and highly available.
    

### How It Works

- **Setup**: You choose the directory type that best fits your needs and set it up through the AWS Management Console. The setup involves specifying directory details such as domain name, admin password, and VPC settings.
    
- **Management**: AWS manages the infrastructure for the directory, handling things like database backups, patch management, and high availability.
    
- **Integration**: Once the directory is active, you can integrate it with other AWS services. For example, you can join Amazon EC2 instances to a directory, authorize AWS Management Console access, or manage access to applications running on AWS.
    
- **Maintenance and Monitoring**: AWS provides monitoring tools through Amazon CloudWatch and also handles maintenance tasks like software patching, thus reducing the administrative burden on your IT teams.
    

### Benefits

- **Simplified Management**: AWS handles much of the heavy lifting of directory maintenance, from backups to software updates.
    
- **Scalability**: Easily scales to meet the needs of your organization as it grows.
    
- **Security and Compliance**: Built with compliance and security in mind, ensuring that your directory services align with industry standards.
    
- **Hybrid Environment Support**: Supports hybrid environments that bridge your on-premises deployments with the cloud, making it ideal for gradual cloud migrations.
    

### Use Cases

- **Single Sign-On (SSO)**: Facilitates SSO to AWS services and business applications, improving user experience and security.
    
- **User and Group Management**: Manages user accounts and group permissions, streamlining access control across AWS services.
    
- **Directory-aware Workloads**: Supports applications that require LDAP or Active Directory for authentication and authorization, such as Microsoft SharePoint or custom .NET applications on EC2.
    

AWS Directory Service is a key component for businesses leveraging AWS cloud resources that require robust, scalable directory services integrated with their cloud and on-premises environments. Whether you are fully cloud-native or operating in a hybrid setup, AWS Directory Service offers a range of options to support different directory requirements effectively.