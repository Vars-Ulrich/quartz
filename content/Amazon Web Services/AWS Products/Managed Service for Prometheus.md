---
sticker: vault//Media/icons/aws-icons/ManagedServiceForPrometheus.svg
---
# Overview

AWS Managed Service for Prometheus is a fully managed Prometheus-compatible monitoring and alerting service offered by Amazon Web Services. Prometheus is a popular open-source monitoring system and time series database widely used in cloud-native environments, particularly those that use container orchestration systems like Kubernetes. AWS Managed Service for Prometheus is designed to make it easier for DevOps teams and developers to securely monitor containerized applications at scale without having to manage the underlying infrastructure.

### Key Features of AWS Managed Service for Prometheus

1. **Fully Managed**: AWS takes care of the provisioning, setup, scaling, and maintenance of your Prometheus monitoring environment, allowing you to focus on monitoring your applications rather than managing the infrastructure.
    
2. **Scalability**: The service is built to automatically scale based on the monitoring workload, which means it can handle large volumes of metrics data without the need for manual intervention.
    
3. **Secure**: Integrates with AWS Identity and Access Management (IAM) to manage access to the service securely. It also supports data encryption at rest and in transit.
    
4. **Compatibility with Prometheus**: Offers full compatibility with open-source Prometheus, which means you can use the same Prometheus Query Language (PromQL) that you use in your existing Prometheus setups.
    
5. **Seamless Integration with AWS Services**: Integrates with AWS container services such as Amazon Elastic Kubernetes Service (EKS) and Amazon Elastic Container Service (ECS), as well as AWS Lambda, allowing for comprehensive monitoring of these services.
    
6. **Managed Alerting**: Supports Prometheus alerting rules, enabling you to define alerts that notify you about issues in your environment through services like Amazon Simple Notification Service (SNS).
    

### How It Works

- **Setup and Configuration**: You can set up and configure the AWS Managed Service for Prometheus directly from the AWS Management Console. This includes creating workspaces, which are isolated environments where your monitoring data is stored.
    
- **Data Collection**: Configure your applications to send metrics to the service. If you're using Kubernetes, you can deploy Prometheus exporters in your cluster, which will collect metrics and send them to your Prometheus workspace.
    
- **Query and Monitor**: Use PromQL to query the metrics data. You can create dashboards using Amazon Managed Grafana (a separate service) or other Grafana instances to visualize the metrics and gain insights into the performance of your applications.
    
- **Alert Configuration**: Define alerting rules based on the metrics you are collecting. These rules can trigger notifications through integrated AWS services like Amazon SNS, helping you respond to potential issues swiftly.
    

### Benefits

- **Reduced Operational Overhead**: By offloading the management of the monitoring infrastructure, you save time and resources that would otherwise be spent on installation, scaling, and maintenance.
    
- **Enhanced Scalability and Reliability**: The service is designed to handle high volumes of data and provides the reliability expected from AWS infrastructure.
    
- **Security and Compliance**: Leverages AWS security features, ensuring that your monitoring setup complies with the stringent security standards of AWS.
    

### Use Cases

- **Container Monitoring**: Ideal for monitoring applications running in containerized environments, particularly those managed using Kubernetes.
    
- **Application Performance Monitoring (APM)**: Track application performance and resource usage to identify bottlenecks and optimize resource allocation.
    
- **Infrastructure Health Monitoring**: Monitor the health and performance of a wide range of infrastructure components across cloud and hybrid environments.
    

AWS Managed Service for Prometheus provides a robust, scalable, and secure environment for monitoring containerized applications, making it an excellent choice for enterprises adopting modern DevOps practices and cloud-native technologies.