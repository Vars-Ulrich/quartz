---
icon: AiFileCache
---
# Overview

### Service Overview:

AWS FileCache is a managed file caching service that enables organizations to accelerate data access and improve performance for on-premises applications and workloads by caching frequently accessed files and objects from Amazon S3, Amazon EFS, or other AWS storage services. It provides a scalable and cost-effective solution for optimizing data access latency and reducing network bandwidth consumption for distributed applications and users.

### Key Features:

1. **Automatic File Caching**: FileCache automatically caches frequently accessed files and objects from [[Simple Storage Service|Amazon S3]], [[Elastic File System|Amazon EFS]], or other AWS storage services on local storage appliances or edge devices, reducing latency and improving data access performance.
2. **Intelligent Caching Policies**: FileCache supports configurable caching policies based on file access patterns, file size, and storage capacity, allowing organizations to optimize cache utilization and eviction policies for specific workloads and applications.
3. **Transparent Integration**: FileCache seamlessly integrates with existing on-premises applications and workflows, requiring no application or code changes, with transparent file access redirection and caching performed at the network layer.
4. **Dynamic Cache Sizing**: FileCache dynamically adjusts cache sizes and eviction policies based on workload demands and storage capacity constraints, ensuring optimal cache performance and efficiency without manual intervention.
	1. **Data Consistency and Coherency**: FileCache ensures data consistency and coherency between cached files and objects and their corresponding sources in [[Simple Storage Service|Amazon S3]] or [[Elastic File System|Amazon EFS]], with support for cache invalidation, synchronization, and data integrity checks.
5. **High Availability and Fault Tolerance**: FileCache provides high availability and fault tolerance features, with support for active-passive or active-active deployment configurations, automatic failover, and data replication for resilience against hardware failures and outages.
6. **Data Encryption and Security**: FileCache encrypts data in transit and at rest using industry-standard encryption protocols, ensuring data security and confidentiality during transfer and storage on local cache appliances or edge devices.
7. **Centralized Management**: FileCache offers centralized management and monitoring capabilities through the [[Management Console]] or [[Application Programming Interface|APIs]], allowing administrators to configure, deploy, and monitor FileCache instances and cache performance metrics.
8. **Cost Optimization**: FileCache offers a pay-as-you-go pricing model with no upfront fees or long-term commitments, allowing organizations to pay only for the cache storage capacity and data transfer resources they consume, with cost optimization features such as tiered pricing and usage-based billing.

### How It Works:

1. **Cache Deployment**: Administrators deploy FileCache appliances or edge devices on-premises within the organization's network infrastructure, configuring them to connect to Amazon S3, Amazon EFS, or other AWS storage services.
2. **Cache Configuration**: Administrators configure caching policies, cache sizes, eviction policies, and access controls for FileCache instances, optimizing cache performance and resource utilization for specific workloads and applications.
3. **Data Access Redirection**: FileCache intercepts file access requests from on-premises applications and users, redirecting requests for cached files and objects to the local cache appliances or edge devices, minimizing latency and network bandwidth usage.
4. **Cache Population**: FileCache automatically populates the cache with frequently accessed files and objects from Amazon S3, Amazon EFS, or other AWS storage services, prefetching data based on access patterns and caching policies to improve cache hit rates.
5. **Data Consistency and Coherency**: FileCache ensures data consistency and coherency between cached files and objects and their corresponding sources in AWS storage services, with support for cache invalidation, synchronization, and data integrity checks.
6. **Cache Monitoring and Management**: Administrators monitor and manage FileCache instances using the AWS Management Console or APIs, accessing cache performance metrics, log files, and status updates to troubleshoot issues and optimize cache performance.
7. **Scalability and Elasticity**: FileCache scales automatically to accommodate growing data volumes and user demands, with support for adding additional cache appliances or edge devices as needed, ensuring elastic and scalable caching infrastructure.
8. **Data Encryption and Security**: FileCache encrypts data in transit and at rest using industry-standard encryption protocols, ensuring data security and confidentiality during transfer and storage on local cache appliances or edge devices.

### Benefits:

1. **Improved Performance**: FileCache accelerates data access and improves application performance by caching frequently accessed files and objects locally, reducing latency and minimizing network bandwidth consumption for distributed applications and users.
2. **Scalability and Elasticity**: FileCache scales automatically to accommodate growing data volumes and user demands, with support for adding additional cache appliances or edge devices as needed, ensuring elastic and scalable caching infrastructure.
3. **Cost Optimization**: FileCache offers a pay-as-you-go pricing model with no upfront fees or long-term commitments, allowing organizations to pay only for the cache storage capacity and data transfer resources they consume, with cost optimization features such as tiered pricing and usage-based billing.
4. **Data Security and Compliance**: FileCache encrypts data in transit and at rest using industry-standard encryption protocols, ensuring data security and confidentiality during transfer and storage on local cache appliances or edge devices, with support for compliance requirements such as HIPAA and GDPR.
5. **Simplified Management**: FileCache provides centralized management and monitoring capabilities through the AWS Management Console or APIs, allowing administrators to configure, deploy, and monitor FileCache instances and cache performance metrics with ease.
6. **Transparent Integration**: FileCache seamlessly integrates with existing on-premises applications and workflows, requiring no application or code changes, with transparent file access redirection and caching performed at the network layer.

### Use Cases:

1. **Content Distribution**: Media and entertainment companies use FileCache to accelerate content distribution and delivery by caching frequently accessed media files and streaming content locally, reducing latency and improving user experience.
2. **Edge Computing**: Organizations deploy FileCache at edge locations to cache data locally for IoT devices, sensors, and edge applications, enabling low-latency data access and processing without
