---
icon: AiGlobalAccelerator
---
# Global Accelerator
AWS Global Accelerator is a service that improves the availability and performance of your applications with local or global users. It provides static IP addresses that act as a fixed entry point to your application endpoints in a single or multiple AWS Regions, such as your Application Load Balancers, Network Load Balancers, or Amazon EC2 instances. AWS Global Accelerator uses the AWS global network to optimize the path from your users to your applications, improving the performance of your traffic by as much as 60%.

Global Accelerator improves performance for a wide range of applications over TCP or UDP by proxying packets at the edge to applications running in one or more AWS Regions. Global Accelerator is a good fit for non-HTTP use cases, such as gaming (UDP), IoT (MQTT), or Voice over IP, as well as for [[Hypertext Transfer Protocol|HTTP]] use cases that specifically require static IP addresses or deterministic, fast regional failover.

#### Exam Alerts
- Please review the differences between CloudFront and Global Accelerator: https://aws.amazon.com/global-accelerator/faqs