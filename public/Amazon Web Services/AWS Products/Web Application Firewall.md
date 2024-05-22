---
icon: AiWAF
aliases:
  - WAF
---
# Overview
- a web app firewall allowing for  monitoring of [[Hypertext Transfer Protocol|HTTP]] reqs that are forwarded to:
	- a [[CloudFront]] distro
	- an [[API Gateway]] [[Application Programming Interface|API]]
	- an [[Elastic Load Balancing#Application load balancer|Application Load Balancer]]
### Pricing
- Charges based on:


### Service Overview:

AWS WAF (Web Application Firewall) is a managed security service provided by Amazon Web Services (AWS) that helps protect web applications from common web exploits, such as SQL injection, cross-site scripting (XSS), and DDoS attacks. AWS WAF allows customers to create custom web security rules and policies to filter and monitor incoming HTTP/HTTPS traffic to their web applications deployed on AWS or on-premises.

### Key Features:

1. **Web Security Rules**: AWS WAF enables customers to define custom rules and conditions to inspect and filter incoming web traffic based on characteristics such as IP addresses, HTTP headers, request methods, query strings, and request payloads.
2. **Managed Rule Sets**: AWS WAF provides pre-configured rule sets developed by AWS and third-party security experts to address common security threats and compliance requirements, such as the OWASP Top 10 vulnerabilities and AWS Managed Rules for AWS-specific protections.
3. **Rate Limiting and Bot Control**: AWS WAF allows customers to set rate-based rules to limit the number of requests from a client IP address or to detect and block malicious bot traffic, helping to prevent DDoS attacks and protect web server resources.
4. **Geo-IP Blocking**: AWS WAF supports geo-location-based rules to block or allow traffic from specific countries or regions, enabling customers to enforce access controls and comply with regulatory requirements.
5. **Integration with AWS Services**: AWS WAF integrates seamlessly with other AWS services such as Amazon CloudFront, Amazon API Gateway, AWS Application Load Balancer (ALB), and AWS Shield Advanced, providing comprehensive protection for web applications deployed in AWS environments.
6. **Logging and Monitoring**: AWS WAF provides detailed logging of web requests and security events, including allowed requests, blocked requests, and compliance violations, which can be analyzed using Amazon CloudWatch Logs and Amazon Athena for security monitoring and forensic analysis.
7. **Customization and Flexibility**: AWS WAF offers a flexible and customizable architecture, allowing customers to create and manage web security rules using AWS Management Console, AWS CLI, or AWS CloudFormation templates, and to update rules dynamically in real-time.
8. **Scalability and Performance**: AWS WAF is designed to scale automatically to handle large volumes of web traffic and to provide low-latency processing of HTTP/HTTPS requests, ensuring high availability and performance for web applications.
9. **Cost-Effective**: AWS WAF offers a pay-as-you-go pricing model with no upfront costs or long-term commitments, allowing customers to pay only for the resources and traffic processed by the service, which helps to reduce operational costs and optimize security budgets.
10. **Compliance and Governance**: AWS WAF helps customers meet industry-specific compliance requirements, such as PCI DSS, HIPAA, GDPR, and SOC 2, by providing granular controls, audit trails, and security documentation for web application security.

### How It Works:

1. **Web ACL Creation**: Customers create a Web Access Control List (ACL) in AWS WAF to define the security rules and policies for filtering and monitoring web traffic to their applications.
2. **Rule Configuration**: Customers configure custom rules and conditions within the Web ACL to inspect and filter incoming HTTP/HTTPS requests based on various criteria, such as IP addresses, headers, query strings, and request payloads.
3. **Managed Rule Sets**: Customers can choose to enable pre-configured rule sets provided by AWS or third-party vendors to address specific security threats and compliance requirements without having to create custom rules from scratch.
4. **Rule Evaluation**: When a web request is received by the application, AWS WAF evaluates the request against the configured rules in the Web ACL and takes action based on the matching conditions, such as allowing, blocking, or logging the request.
5. **Logging and Monitoring**: AWS WAF logs detailed information about each web request and security event, including the rule that matched the request, the action taken, and additional metadata, which can be analyzed in real-time using Amazon CloudWatch Logs or stored for later analysis.
6. **Integration with AWS Services**: AWS WAF integrates with other AWS services such as Amazon CloudFront, Amazon API Gateway, AWS Application Load Balancer (ALB), and AWS Shield Advanced to provide comprehensive protection for web applications deployed in AWS environments.
7. **Continuous Improvement**: Customers can continuously monitor and fine-tune their Web ACLs based on security insights and analytics to adapt to evolving threats and compliance requirements and to optimize the performance and effectiveness of their web application security posture.

### Benefits:

1. **Enhanced Security**: AWS WAF helps protect web applications from common web exploits and attacks, such as SQL injection, XSS, and DDoS, by allowing customers to create custom security rules and policies tailored to their specific security requirements.
2. **Compliance and Governance**: AWS WAF helps customers meet industry-specific compliance requirements, such as PCI DSS, HIPAA, GDPR, and SOC 2, by providing granular controls, audit trails, and security documentation for web application security.
3. **Improved Performance**: AWS WAF provides low-latency processing of HTTP/HTTPS requests and scalable infrastructure to handle large volumes of web traffic, ensuring high availability and performance for web applications.
4. **Cost Optimization**: AWS WAF offers a pay-as-you-go pricing model with no upfront costs or long-term commitments, allowing customers to pay only for the resources and traffic processed by the service, which helps to reduce operational costs and optimize security budgets.
5. **Simplified Management**: AWS WAF offers a user-friendly interface and API for creating, configuring, and managing web security rules and policies, enabling customers to streamline security operations and respond quickly to security events and incidents.

### Use Cases:

1. **Web Application Security**: AWS WAF is used to protect web applications hosted on AWS or on-premises from common web exploits and attacks, such as SQL injection, XSS, and DDoS, by filtering and monitoring incoming HTTP/HTTPS traffic.
2. **API Security**: AWS WAF is used to secure APIs and microservices deployed on Amazon API Gateway by filtering and monitoring incoming API requests, enforcing access controls, and protecting against malicious attacks and abuse.
3. **Content Delivery Networks (CDNs)**: AWS WAF is used to enhance the security of content delivery networks (CDNs) such as Amazon CloudFront by filtering and blocking malicious traffic at the edge, reducing the risk of DDoS attacks and unauthorized access.
4. **Compliance Enforcement**: AWS WAF is used to enforce compliance requirements, such as PCI DSS and HIPAA, by applying security controls and access policies to web applications and APIs to protect sensitive data and ensure regulatory compliance.
5. **Threat Intelligence Integration**: AWS WAF is used to integrate with threat intelligence feeds and security automation tools to enhance threat detection and response capabilities, enabling proactive security measures and real-time incident response.
6. **Application Visibility and Logging**: AWS WAF is used to gain visibility into web traffic patterns, security events, and compliance violations by logging detailed information about each web request and security event, which can be analyzed for security monitoring and forensic analysis.