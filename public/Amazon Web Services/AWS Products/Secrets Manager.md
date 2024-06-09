---
icon: AiSecretsManager
aliases:
  - AWS Secrets Manager
---
# Overview 
- helps you protect secrets needed to access your applications services and IT resources
- Enables easy rotation, management, and retrieval of database credentials, [[Application Programming Interface|API]] and other secrets throughout their lifecycle
- 
### Price
- charges based on:
	- Number of secrets stored
	- [[Application Programming Interface|API]] calls made

AWS Secrets Manager is a fully managed service that helps you securely store, manage, and rotate secrets such as API keys, passwords, database credentials, and other sensitive information used by your applications and services. It provides a centralized and secure repository for managing secrets, with built-in encryption, access controls, and automated rotation capabilities to enhance security and compliance.

### Key Features:

1. **Secret Storage**: Secrets Manager provides a secure and centralized repository for storing secrets, ensuring sensitive information is encrypted at rest and in transit.
2. **Secret Rotation**: Secrets Manager automates the rotation of secrets, such as database passwords and API keys, to help maintain security and compliance with best practices.
3. **Integration with AWS Services**: Secrets Manager seamlessly integrates with other AWS services, allowing you to securely access and manage secrets from EC2 instances, Lambda functions, RDS databases, and more.
4. **Fine-Grained Access Controls**: Secrets Manager offers fine-grained access controls, allowing you to define policies to control who can access, manage, and rotate secrets within your AWS environment.
5. **Audit Logging**: Secrets Manager provides audit logging capabilities to track access and changes to secrets, helping you meet compliance requirements and monitor security incidents.
6. **Automatic Encryption**: Secrets Manager automatically encrypts secrets using AWS Key Management Service (KMS), ensuring data confidentiality and integrity.
7. **High Availability and Durability**: Secrets Manager is designed for high availability and durability, with built-in replication and backup mechanisms to ensure secrets are always accessible and protected.
8. **Secure Secret Retrieval**: Secrets Manager provides secure APIs and client libraries for retrieving secrets programmatically, ensuring sensitive information is protected during transmission.

### How It Works:

1. **Secret Creation**: You create secrets in Secrets Manager by specifying the secret value (e.g., password, API key) and optional metadata (e.g., description, tags) through the AWS Management Console, API, or CLI.
2. **Secret Rotation**: You configure automatic rotation for supported types of secrets (e.g., RDS database passwords, IAM credentials) using Secrets Manager's rotation functionality, which automatically generates and updates secret values on a schedule.
3. **Access Controls**: You define IAM policies to control access to secrets, specifying which users, roles, or services are allowed to retrieve, update, or rotate secrets within your AWS environment.
4. **Integration**: You integrate Secrets Manager with your applications and services by using AWS SDKs, CLI commands, or client libraries, which provide secure APIs for retrieving and managing secrets programmatically.
5. **Audit Logging**: You enable audit logging in Secrets Manager to track access and changes to secrets, allowing you to monitor and audit activity within your AWS environment for compliance and security purposes.

### Benefits:

1. **Enhanced Security**: Secrets Manager helps you improve security by centralizing and encrypting sensitive information, enforcing access controls, and automating secret rotation to reduce the risk of data breaches.
2. **Simplified Management**: Secrets Manager simplifies the management of secrets by providing a single, centralized repository for storing and accessing sensitive information, reducing operational overhead and complexity.
3. **Automated Rotation**: Secrets Manager automates the rotation of secrets, reducing the risk of credential compromise and ensuring compliance with security best practices and regulatory requirements.
4. **Integration with AWS Services**: Secrets Manager seamlessly integrates with other AWS services, allowing you to securely access and manage secrets from your applications, databases, serverless functions, and other AWS resources.
5. **Audit Logging and Monitoring**: Secrets Manager provides audit logging and monitoring capabilities to track access and changes to secrets, helping you meet compliance requirements and detect security incidents.
6. **Cost-Effective**: Secrets Manager offers a pay-as-you-go pricing model based on the number of secrets stored and API requests made, allowing you to pay only for what you use without upfront commitments or long-term contracts.

### Use Cases:

1. **Database Credentials**: Store and manage database credentials (e.g., usernames, passwords) securely in Secrets Manager and automate the rotation of database passwords to enhance security.
2. **API Keys and Tokens**: Store and manage API keys, access tokens, and other authentication credentials used by your applications and services, ensuring sensitive information is protected and rotated regularly.
3. **SSH Keys**: Store and manage SSH keys used for secure access to servers and instances, enforcing access controls and automated rotation to reduce the risk of unauthorized access.
4. **Encryption Keys**: Store and manage encryption keys and other cryptographic materials used for data encryption and decryption, ensuring data confidentiality and integrity in your applications and services.

AWS Secrets Manager provides a secure, scalable, and fully managed solution for storing, managing, and rotating secrets in your AWS environment, helping you improve security, simplify management, and meet compliance requirements for sensitive information.