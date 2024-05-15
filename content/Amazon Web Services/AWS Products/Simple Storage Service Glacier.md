---
sticker: vault//Media/icons/aws-icons/SimpleStorageServiceGlacier.svg
aliases:
  - S3 Glacier
---
# Overview

Amazon Simple Storage Service (S3) Glacier is an archival storage solution within Amazon S3 designed for data archiving and long-term storage at a lower cost. It allows you to store data that is infrequently accessed and doesn't require immediate retrieval, making it ideal for backup, compliance, and regulatory requirements.

### Key Features:

1. **Archival Storage**: S3 Glacier provides archival storage for data that is not frequently accessed and requires long-term retention.
2. **Low Cost**: Glacier offers lower storage costs compared to standard S3 storage classes, making it cost-effective for storing large volumes of data over extended periods.
3. **Data Retrieval Options**: Glacier offers different retrieval options, including expedited, standard, and bulk retrievals, with varying costs and retrieval times.
4. **Flexible Storage Classes**: Glacier offers multiple storage classes, including Glacier (S3 Glacier) and Glacier Deep Archive (S3 Glacier Deep Archive), allowing you to choose the appropriate storage class based on your data access requirements and budget.
5. **Data Durability and Availability**: Glacier provides the same level of durability and availability as standard S3 storage, ensuring that your data is protected against hardware failures and is available when needed.

### How It Works:

1. **Upload Data**: You can upload data to S3 Glacier using the AWS Management Console, AWS CLI, or SDKs. Once uploaded, the data is stored securely in Glacier's archival storage.
2. **Retrieve Data**: To retrieve data from Glacier, you initiate a retrieval request specifying the retrieval option (expedited, standard, or bulk). Glacier then retrieves the requested data and makes it available for download within the specified retrieval time.
3. **Data Lifecycle Policies**: You can set lifecycle policies to automatically transition data from standard S3 storage classes to Glacier based on predefined rules, helping you optimize storage costs and manage data lifecycle efficiently.
4. **Vaults and Archives**: In Glacier, data is organized into vaults, which act as containers for storing archives. Each archive represents a single data object that can be retrieved or deleted individually.
5. **Data Encryption**: Glacier encrypts data at rest using server-side encryption (SSE), ensuring that your data is encrypted and protected while stored in archival storage.

### Benefits:

1. **Cost-Effective Storage**: Glacier offers lower storage costs compared to standard S3 storage classes, making it an economical choice for long-term data retention.
2. **Compliance and Regulatory Requirements**: Glacier helps you meet compliance and regulatory requirements for data retention and archival storage, providing durable and secure storage for sensitive data.
3. **Scalability and Durability**: Glacier provides scalable and durable storage, allowing you to store large volumes of data securely and reliably over extended periods.
4. **Data Lifecycle Management**: Glacier integrates with S3 lifecycle policies, allowing you to automate data lifecycle management and transition data between storage classes based on predefined rules.
5. **Flexible Retrieval Options**: Glacier offers flexible retrieval options with varying costs and retrieval times, allowing you to choose the option that best fits your data access requirements and budget.

### Use Cases:

1. **Data Archiving**: Store backup and archival data in Glacier for long-term retention and compliance with regulatory requirements.
2. **Digital Preservation**: Preserve digital assets such as documents, images, and historical records in Glacier for future access and reference.
3. **Compliance and Regulatory Compliance**: Store records, logs, and audit trails in Glacier to meet compliance and regulatory requirements for data retention and archival storage.
4. **Disaster Recovery**: Use Glacier as part of your disaster recovery strategy to store backup copies of critical data and ensure data availability in the event of a disaster or data loss.
5. **Media and Entertainment**: Archive media files, videos, and digital assets in Glacier for long-term storage and preservation, reducing storage costs and freeing up space in primary storage systems.

Amazon S3 Glacier provides a cost-effective and durable solution for archival storage, enabling you to store large volumes of data securely and reliably for long-term retention and compliance requirements. With flexible storage classes, retrieval options, and data lifecycle management capabilities, Glacier helps you optimize storage costs, meet regulatory requirements, and ensure data availability when needed.