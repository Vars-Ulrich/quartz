---
sticker: vault//Media/icons/aws-icons/SimpleQueueService.svg
aliases:
  - SQS
---
# Overview

https://tutorialsdojo.com/amazon-sqs
long polling

Three main parts of a distributed messaging system

1 Components of dist. system (instances)

2 The queue (dist on Amazon SQS servers)

3 Messages in the queue

### Service Overview:

Amazon Simple Queue Service (SQS) is a fully managed message queuing service that enables you to decouple and scale microservices, distributed systems, and serverless applications. It provides a reliable, scalable, and cost-effective way to send, store, and process messages between components of your applications.

### Key Features:

1. **Message Queues**: SQS allows you to create message queues that act as temporary storage for messages sent between components of your applications.
2. **Fully Managed**: SQS is a fully managed service, which means AWS handles the operational aspects of provisioning, scaling, and maintaining the infrastructure for message queues.
3. **Distributed Architecture**: SQS is designed to be distributed and highly available, ensuring that messages are reliably stored and delivered across multiple Availability Zones.
4. **Multiple Queue Types**: SQS offers two types of message queues: Standard Queues, which provide best-effort ordering and at-least-once message delivery, and FIFO (First-In-First-Out) Queues, which guarantee exactly-once processing and message ordering.
5. **Message Retention**: SQS allows you to specify the retention period for messages in a queue, ensuring that messages are available for processing within the specified timeframe.
6. **Message Visibility Timeout**: SQS provides a visibility timeout mechanism that temporarily hides messages from other consumers while they are being processed by a single consumer, preventing duplicate processing.
7. **Dead-Letter Queues**: SQS supports dead-letter queues, which capture messages that cannot be processed successfully after a certain number of retries, allowing you to troubleshoot and analyze processing failures.
8. **Integration with AWS Services**: SQS seamlessly integrates with other AWS services such as AWS Lambda, Amazon EC2, Amazon SNS, and Amazon CloudWatch, enabling you to build scalable and fault-tolerant architectures.

### How It Works:

1. **Create Queues**: You can create SQS queues using the AWS Management Console, AWS CLI, or SDKs. Each queue has a unique URL and configurable settings such as message retention period and visibility timeout.
2. **Send Messages**: Applications can send messages to SQS queues using the SendMessage API. Messages can be up to 256 KB in size and can contain metadata such as message attributes.
3. **Receive Messages**: Consumers (or workers) retrieve messages from SQS queues using the ReceiveMessage API. Messages are returned to the consumer along with a unique receipt handle.
4. **Process Messages**: Consumers process the messages retrieved from the queue and delete them using the DeleteMessage API once they have been successfully processed.
5. **Scale Automatically**: SQS automatically scales based on the volume of messages in the queue, ensuring high availability and low latency even under varying workloads.

### Benefits:

1. **Decoupling**: SQS helps decouple the components of your applications, allowing them to operate independently and asynchronously.
2. **Scalability**: SQS scales seamlessly to handle any volume of message traffic, from a few messages per second to millions of messages per day.
3. **Reliability**: SQS provides a highly reliable message delivery mechanism, with built-in redundancy and fault tolerance across multiple Availability Zones.
4. **Cost-Effective**: SQS offers a pay-as-you-go pricing model with no upfront costs or long-term commitments, making it cost-effective for applications of any size.
5. **Easy Integration**: SQS integrates seamlessly with other AWS services and external systems, allowing you to build flexible and scalable architectures.
6. **Operational Efficiency**: With SQS, you can offload the operational overhead of managing message queues to AWS, allowing you to focus on building and improving your applications.

### Use Cases:

1. **Asynchronous Communication**: Use SQS to decouple the components of your applications and enable asynchronous communication between them.
2. **Message Processing**: Use SQS to buffer requests and messages between different parts of your application, ensuring smooth and efficient message processing.
3. **Task Queues**: Use SQS as a task queue to distribute and process workloads across multiple workers or instances in a distributed system.
4. **Event-Driven Architectures**: Use SQS in conjunction with AWS Lambda or Amazon SNS to build event-driven architectures that respond to events and triggers in real time.
5. **Batch Processing**: Use SQS to implement batch processing workflows for handling large volumes of data and processing tasks in parallel.

Amazon SQS is a powerful and versatile messaging service that enables you to build scalable, decoupled, and reliable applications in the AWS cloud. Whether you're building microservices, distributed systems, or serverless applications, SQS provides a simple and cost-effective way to manage message queues and process messages at any scale.
