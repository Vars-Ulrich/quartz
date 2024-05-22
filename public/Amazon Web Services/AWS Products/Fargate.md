---
icon: AiFargate
---
# Fargate
AWS Fargate is a serverless compute engine for containers. It works with both Amazon Elastic Container Service (ECS) and Amazon Elastic Kubernetes Service (EKS). Fargate makes it easy for you to focus on building your applications. Fargate removes the need to provision and manage servers, lets you specify and pay for resources per application, and improves security through application isolation by design. Fargate allocates the right amount of compute, eliminating the need to choose instances and scale cluster capacity. You only pay for the resources required to run your containers, so there is no over-provisioning and paying for additional servers. Fargate runs each task or pod in its kernel providing the tasks and pods their own isolated compute environment. This enables your application to have workload isolation and improved security by design.

### Service Overview:

AWS Fargate is a serverless compute engine for containers that allows you to run containers without having to manage the underlying infrastructure. It abstracts away the complexities of provisioning and managing servers, enabling you to focus solely on deploying and managing your containerized applications. With Fargate, you can deploy containers in a fully managed environment, eliminating the need to provision and manage virtual machines or clusters.

### Key Features:

1. **Serverless Computing**: Fargate provides a serverless compute environment for running containers, allowing you to deploy and scale containerized applications without managing underlying servers or clusters.
2. **Container Orchestration**: Fargate seamlessly integrates with container orchestration services like Amazon ECS (Elastic Container Service) and Amazon EKS (Elastic Kubernetes Service), enabling you to deploy, manage, and scale containerized applications using familiar orchestration tools and APIs.
3. **Resource Isolation**: Fargate provides resource isolation for containers, ensuring that each container gets its allocated CPU and memory resources, preventing noisy neighbor issues and resource contention.
4. **Automatic Scaling**: Fargate automatically scales your containerized applications based on demand, allowing you to handle fluctuations in traffic and workload without manual intervention.
5. **Pay-per-Use Pricing**: Fargate follows a pay-per-use pricing model, where you only pay for the vCPU and memory resources consumed by your containers, providing cost efficiency and eliminating the need for over-provisioning.
6. **Built-in Security**: Fargate provides built-in security features such as isolation between containers, encryption at rest and in transit, and integration with AWS Identity and Access Management (IAM) for fine-grained access control.
7. **High Availability**: Fargate ensures high availability for your containerized applications by automatically distributing containers across multiple Availability Zones within a region, providing fault tolerance and resiliency.
8. **Integration with AWS Services**: Fargate seamlessly integrates with other AWS services such as Amazon VPC (Virtual Private Cloud), AWS CloudFormation, AWS CodeDeploy, AWS CloudWatch, and AWS CloudTrail, enabling you to leverage the full capabilities of the AWS ecosystem.
9. **Managed Updates**: Fargate manages updates and patches for the underlying infrastructure, ensuring that your containerized applications are always running on the latest and most secure platform version.
10. **Container Networking**: Fargate provides integrated networking capabilities for containers, allowing them to communicate with each other within the same task or across multiple tasks, and with other AWS services over private or public networks.

### How It Works:

1. **Container Definition**: You define your containerized applications using container images stored in container registries such as Amazon ECR (Elastic Container Registry) or Docker Hub, specifying container configurations, resource requirements, and networking settings.
2. **Task Definition**: You define tasks using Task Definitions in Amazon ECS or Kubernetes Pods in Amazon EKS, specifying the containers to run, their configurations, dependencies, and resource requirements.
3. **Cluster Management**: Fargate automatically provisions and manages the underlying infrastructure needed to run your containerized applications, including compute resources, networking, and storage.
4. **Task Scheduling**: Fargate schedules tasks onto the available compute resources based on resource requirements, availability, and constraints, ensuring optimal resource utilization and performance.
5. **Container Execution**: Fargate launches and manages containers based on the specifications defined in the Task Definition, ensuring that each container gets its allocated CPU and memory resources and that they run in isolation from each other.
6. **Automatic Scaling**: Fargate automatically scales your containerized applications based on CPU and memory utilization, allowing you to handle changes in workload and demand without manual intervention.
7. **Monitoring and Logging**: Fargate integrates with AWS CloudWatch for monitoring container metrics, logs, and alarms, providing visibility into the performance and health of your containerized applications.
8. **Security and Compliance**: Fargate provides built-in security features such as encryption, IAM integration, and network isolation, ensuring that your containerized applications are secure and compliant with regulatory requirements.
9. **Integration with CI/CD Pipelines**: Fargate seamlessly integrates with CI/CD pipelines and deployment tools such as AWS CodePipeline, AWS CodeBuild, and AWS CodeDeploy, enabling automated deployment and continuous delivery of containerized applications.
10. **Cost Optimization**: Fargate helps optimize costs by providing granular visibility and control over resource utilization, allowing you to right-size your containerized applications and only pay for the resources consumed.

### Benefits:

1. **Simplicity**: Fargate simplifies the deployment and management of containerized applications by abstracting away the underlying infrastructure, allowing you to focus on application development and deployment.
2. **Scalability**: Fargate automatically scales your containerized applications based on demand, ensuring that you can handle changes in workload and traffic without manual intervention or over-provisioning.
3. **Cost Efficiency**: Fargate follows a pay-per-use pricing model, where you only pay for the vCPU and memory resources consumed by your containers, providing cost efficiency and eliminating the need for over-provisioning.
4. **Operational Efficiency**: Fargate streamlines operations by managing the underlying infrastructure, updates, and patches for you, reducing operational overhead and allowing you to focus on building and delivering applications.
5. **Security and Compliance**: Fargate provides built-in security features and integration with AWS services such as IAM and AWS Key Management Service (KMS), ensuring that your containerized applications are secure and compliant with regulatory requirements.
6. **Flexibility**: Fargate supports both Amazon ECS and Amazon EKS, giving you the flexibility to choose the container orchestration service that best fits your requirements and preferences.
7. **High Availability**: Fargate ensures high availability for your containerized applications by automatically distributing containers across multiple Availability Zones within a region, providing fault tolerance and resiliency.
8. **Integration with AWS Services**: Fargate seamlessly integrates with other AWS services, enabling you to leverage the full capabilities of the AWS ecosystem for building, deploying, and managing containerized applications.

### Use Cases:

1. **Web Applications**: Fargate is well-suited for hosting web applications, APIs, and microservices, providing a scalable and cost-effective platform for serving dynamic content and handling varying levels of traffic.
2. **Batch Processing**: Fargate can be used for running batch processing jobs, data processing tasks, and ETL (Extract, Transform, Load) workflows, allowing you to process large volumes of data efficiently and cost-effectively.
3. **CI/CD Pipelines**: Fargate integrates seamlessly with CI/CD pipelines, enabling automated deployment and continuous delivery of containerized applications, reducing time-to-market and improving software quality.
4. **Machine Learning Workloads**: Fargate can be used for running machine learning inference workloads, model serving, and data preprocessing tasks, providing a scalable and flexible platform for machine learning deployments.
5. **Dev/Test Environments**: Fargate is ideal for creating development and testing environments, allowing you to quickly provision and manage isolated environments for software development, testing, and debugging.
6. **Event-Driven Workflows**: Fargate can be used for running event-driven workflows, such as event processing pipelines, stream processing, and event-driven microservices, enabling you to build responsive and scalable applications that react to real-time events and triggers.
7. **Containerized Applications**: Fargate is suitable for running a wide range of containerized applications, including web servers, databases, caching servers, message brokers, and more, providing a flexible and scalable platform for deploying and managing containerized workloads.
8. **Stateless Applications**: Fargate is well-suited for stateless applications that can horizontally scale out by adding more instances, such as web servers, API endpoints, and microservices, allowing you to handle increasing levels of traffic and workload.
9. **Scheduled Jobs**: Fargate can be used for running scheduled jobs, cron jobs, and periodic tasks, such as data backups, log rotations, and system maintenance tasks, enabling you to automate routine operations and reduce manual effort.
10. **Multi-Tier Architectures**: Fargate supports multi-tier architectures with front-end, back-end, and data storage components, allowing you to deploy complex applications with separate layers for presentation, business logic, and data storage.
11. **Hybrid Cloud Deployments**: Fargate can be used in hybrid cloud environments, allowing you to seamlessly extend your on-premises infrastructure to the cloud and run containerized workloads across both environments with consistent management and operations.
12. **Batch Processing and Data Analytics**: Fargate is suitable for running batch processing and data analytics workloads, such as data transformation, data warehousing, and data analytics pipelines, enabling you to process and analyze large volumes of data efficiently and cost-effectively.
13. **High-Performance Computing**: Fargate can be used for running high-performance computing (HPC) workloads, such as scientific simulations, rendering, and rendering, providing the compute power and scalability required for computationally intensive tasks.
14. **Internet of Things (IoT) Applications**: Fargate can be used for deploying and managing IoT applications and services, enabling you to process, analyze, and act on data generated by IoT devices in real-time, improving operational efficiency and enabling new use cases.
15. **Content Delivery and Media Streaming**: Fargate can be used for content delivery and media streaming applications, such as video transcoding, content delivery networks (CDNs), and live streaming, providing low-latency and high-throughput processing for multimedia content.

AWS Fargate provides a versatile and scalable platform for deploying and managing containerized applications across a wide range of use cases, enabling organizations to build, deploy, and scale applications quickly and efficiently without managing the underlying infrastructure.