---
sticker: vault//Media/icons/aws-icons/ApplicationDiscoveryService.svg
---
# Overview

AWS Application Discovery Service is a tool provided by Amazon Web Services designed to help enterprise customers plan migration projects by gathering information about their on-premises data centers. This service facilitates the discovery of on-premises server dependencies and network connections, as well as server performance data, helping organizations make informed decisions about migration strategies to the cloud.

### Key Features of AWS Application Discovery Service

1. **Automated Discovery**: The service automatically collects information about your on-premises infrastructure without requiring manual inputs. It can identify servers, storage, networking hardware, and applications running in the data center.
    
2. **Data Collection Methods**: It offers two primary methods for collecting data:
    
    - **Agentless Discovery**: This method uses a virtual appliance to capture high-level data about VMs (virtual machines) and hosts in environments managed through VMware vCenter.
    - **Agent-Based Discovery**: Involves installing lightweight agents on your on-premises servers. These agents collect a more detailed set of data, including configuration, usage, and behavior data about the servers.
3. **Data Visualization and Exporting**: The collected data can be explored within the AWS Management Console, and you can export it for further analysis or to use with other tools like AWS Migration Hub, which helps plan and track the progress of application migrations.
    
4. **Integration with AWS Migration Services**: Integrates with services such as AWS Migration Hub and AWS Cost Explorer to provide comprehensive insights into the potential costs and resources required for a migration project.
    
5. **Secure Data Handling**: Ensures that all collected data is handled securely, adhering to AWS’s stringent security standards.
    

### How It Works

- **Setup**: Depending on the chosen method, you either set up an agentless collector in your environment or install agents on your on-premises servers.
- **Data Collection**: The service begins collecting data about hardware configurations, network dependencies, and application interactions. For agent-based collection, detailed performance metrics and ongoing system activities are also captured.
- **Analysis and Planning**: Use the AWS Application Discovery Service dashboard to analyze the collected data. Understand server utilizations, dependencies, and network traffic patterns to plan your migration effectively.
- **Export Data**: Export the collected data to AWS Migration Hub or use it with third-party tools for a more detailed analysis or as part of your migration plan.

### Benefits

- **Simplifies Migration Planning**: Provides visibility into on-premises environments, which helps in designing effective migration strategies and reduces risks associated with migration projects.
- **Cost Management**: Helps estimate the cost and resource utilization in AWS, allowing for better budgeting and resource allocation.
- **Minimizes Downtime**: By understanding application dependencies and server usages, organizations can strategize their migrations to minimize downtime.

### Use Cases

- **Data Center Decommissioning**: Essential for enterprises looking to migrate their entire data center to the cloud.
- **Application Modernization**: Helps identify and analyze applications for modernization opportunities, such as moving to microservices architecture on AWS.
- **Disaster Recovery Planning**: Enables businesses to plan effective disaster recovery strategies by understanding critical dependencies and server configurations.

AWS Application Discovery Service is particularly valuable for large organizations that require a thorough understanding of their existing IT infrastructure to ensure a smooth and efficient transition to cloud services.