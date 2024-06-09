---
icon: AiCertificateManager
aliases:
  - AWS Certificate Manager
  - ACM
---
# Overview

AWS Certificate Manager (ACM) is a service offered by Amazon Web Services that makes it easier to deploy and manage [[Secure Sockets Layer|SSL]]/[[Transport Layer Security|TLS]] certificates for your AWS-based websites and applications. This service is crucial for securing server communication and ensuring that data transmitted over the internet is encrypted and secure from interception.

### Key Features of AWS Certificate Manager

1. **SSL/TLS Certificate Provisioning**: ACM allows you to easily provision, manage, and deploy public and private Secure Sockets Layer/Transport Layer Security (SSL/TLS) certificates. These certificates are used for securing network communications and establishing the identity of websites over the Internet.
    
2. **Seamless Integration with AWS Services**: ACM certificates can be directly integrated with AWS services such as [[Elastic Load Balancing]], [[CloudFront|Amazon CloudFront]], [[API Gateway|Amazon API Gateway]], and more, allowing you to secure applications easily.
    
3. **Automated Certificate Renewal**: ACM handles the renewal of the SSL/TLS certificates it manages. This automation ensures that the certificates are always valid and reduces the risk of outages due to expired certificates.
    
4. **Centralized Management**: Through the ACM console or the [[Command Line Interface|AWS CLI]], you can manage all your certificates from one place, simplifying the process of deploying, renewing, and managing certificates across various AWS services.
    
5. **Private Certificate Authority**: ACM also includes an option to create a private [[Certificate authority]] (CA) with AWS Certificate Manager Private CA. This private CA can issue certificates used to secure communication within your organization, useful for scenarios where public trust is not required.
    

### How It Works

- **Requesting a Certificate**: You can request a certificate through the ACM console, AWS CLI, or AWS SDK. When requesting a certificate for a domain, ACM will handle the domain validation process to confirm that you own or control the domain.
    
- **Validation Process**: For public certificates, AWS offers DNS validation or email validation. DNS validation is often preferred for its ability to be automated. ACM will provide a CNAME record to be added to your DNS configuration, which AWS uses to validate domain ownership.
    
- **Deployment of Certificates**: Once validated, the certificates can be attached to AWS resources like Elastic Load Balancers, CloudFront distributions, and APIs in API Gateway. The integration process is typically straightforward, involving selecting the ACM certificate from a dropdown menu in the service’s configuration.
    
- **Renewal**: ACM will automatically renew certificates that have been successfully validated using DNS validation. For email validation, you will receive an email when it's time to renew the certificate.
    

### Benefits

- **Enhanced Security**: By facilitating easy deployment of SSL/TLS certificates, ACM helps secure data in transit, enhancing the overall security of your applications.
    
- **Cost-Effective**: There is no additional charge for provisioning or managing SSL/TLS certificates provided by ACM that are used with eligible AWS services.
    
- **Simplified Management**: Automates the complex tasks of certificate provisioning, deployment, and renewal, reducing the administrative overhead traditionally associated with SSL/TLS certificates.
    

### Use Cases

- **Secure Web Applications**: Use ACM to secure user connections to web applications hosted on AWS, ensuring data transmitted is encrypted.
- **Internal Communications**: With ACM Private CA, you can issue certificates to secure internal communications within an AWS environment, such as between microservices or backend systems.
- **Custom Domains with API Gateway**: Secure custom domains for APIs deployed via Amazon API Gateway, providing clients with a secure connection to your APIs.

AWS Certificate Manager is a powerful tool for any organization looking to simplify the management of SSL/TLS certificates while maintaining high levels of security and reliability in their AWS environments.