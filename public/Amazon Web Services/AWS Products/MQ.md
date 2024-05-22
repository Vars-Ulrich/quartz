---
icon: AiMQ
---
# Overview

Amazon MQ - Amazon MQ is a managed message broker service for [[Apache ActiveMQ]] and [[RabbitMQ]] that makes it easy to set up and operate message brokers on AWS. Amazon MQ reduces your operational responsibilities by managing the provisioning, setup, and maintenance of message brokers for you. Because Amazon MQ connects to your current applications with industry-standard APIs and protocols, you can easily migrate to AWS without having to rewrite code.

If you're using messaging with existing applications, and want to move the messaging functionality to the cloud quickly and easily, AWS recommends you consider Amazon MQ. It supports industry-standard APIs and protocols so you can switch from any standards-based message broker to Amazon MQ without rewriting the messaging code in your applications. If you are building brand new applications in the cloud, AWS recommends you consider [[Simple Queue Service|SQS]] and [[Simple Notification Service|Amazon SNS]].
  
Amazon MQ is a managed message broker service provided by Amazon Web Services (AWS) that enables customers to build, operate, and scale message-oriented middleware (MOM) applications in the cloud. It supports industry-standard messaging protocols and provides a reliable, scalable, and fully managed infrastructure for decoupling applications, integrating systems, and implementing asynchronous communication patterns.

### Key Features of Amazon MQ

1. **Compatibility**: Amazon MQ supports popular messaging protocols, including Advanced Message Queuing Protocol (AMQP), Message Queue Telemetry Transport (MQTT), and Java Message Service (JMS). This enables customers to migrate existing messaging applications seamlessly to the cloud.
    
2. **Managed Service**: Amazon MQ is fully managed by AWS, which handles provisioning, scaling, patching, and maintenance of the underlying infrastructure. Customers can focus on building and operating their messaging applications without managing servers or infrastructure.
    
3. **High Availability**: Amazon MQ provides high availability and durability by replicating messages across multiple availability zones (AZs) within a region. This ensures that messages are preserved and accessible even in the event of hardware failures or AZ outages.
    
4. **Scalability**: Amazon MQ scales seamlessly to handle varying workloads and message volumes. It supports horizontal scaling by adding additional brokers and partitions to distribute message processing across multiple instances.
    
5. **Security**: Amazon MQ integrates with AWS Identity and Access Management (IAM) for authentication and access control. It supports encryption at rest and in transit using AWS Key Management Service (KMS) to protect sensitive data and comply with regulatory requirements.
    
6. **Monitoring and Logging**: Amazon MQ provides built-in monitoring and logging capabilities, allowing customers to track message throughput, queue depth, and other metrics using Amazon CloudWatch. It also supports logging to Amazon CloudWatch Logs for auditing and troubleshooting.
    
7. **Integration with AWS Services**: Amazon MQ integrates seamlessly with other AWS services, including AWS Lambda, Amazon S3, Amazon RDS, and Amazon EC2. This allows customers to build event-driven architectures, process messages, and integrate systems across different AWS services.
    

### How It Works

1. **Creating a Broker**: Customers start by creating a message broker instance in Amazon MQ using the AWS Management Console, CLI, or API. They specify configuration settings such as messaging protocol, instance type, and storage capacity.
    
2. **Configuring Access Control**: Customers configure access control policies using IAM to control who can access the message broker and perform operations such as sending, receiving, and deleting messages.
    
3. **Publishing and Subscribing to Messages**: Applications publish messages to Amazon MQ queues or topics using the appropriate messaging protocol and API. Subscribers consume messages from queues or topics and process them asynchronously.
    
4. **Monitoring and Management**: Customers monitor the health and performance of their Amazon MQ brokers using Amazon CloudWatch metrics and alarms. They can adjust configuration settings, scale resources, and troubleshoot issues using the AWS Management Console or API.
    
5. **Integration with Applications**: Amazon MQ integrates with a wide range of applications and development frameworks that support standard messaging protocols such as AMQP, MQTT, and JMS. Customers can use existing messaging clients and libraries to interact with Amazon MQ seamlessly.
    

### Benefits

- **Fully Managed Service**: AWS manages the infrastructure, including provisioning, scaling, and maintenance, reducing operational overhead and allowing customers to focus on building and operating their messaging applications.
    
- **Compatibility and Interoperability**: Amazon MQ supports industry-standard messaging protocols, enabling customers to migrate existing messaging applications to the cloud seamlessly and integrate with a wide range of systems and applications.
    
- **High Availability and Durability**: Amazon MQ provides high availability and durability by replicating messages across multiple AZs within a region, ensuring message availability and reliability even in the event of hardware failures or AZ outages.
    
- **Scalability and Flexibility**: Amazon MQ scales seamlessly to handle varying workloads and message volumes, allowing customers to adjust resources dynamically to meet changing demands and scale their messaging applications as needed.
    
- **Security and Compliance**: Amazon MQ integrates with AWS security services such as IAM and KMS to provide encryption, access control, and compliance with regulatory requirements, ensuring the security and integrity of message data.
    

Amazon MQ is a powerful messaging service that simplifies the deployment, management, and operation of message-oriented middleware applications in the cloud, enabling customers to build scalable, reliable, and resilient messaging solutions with ease.