---
icon: AiAuditManager
---
# Overview

AWS Audit Manager is a service provided by Amazon Web Services designed to help businesses automate the process of auditing their use of AWS services to ensure compliance with regulations or internal policies. This tool simplifies the task of continuous compliance assessments, gathering evidence, and managing audits more efficiently.

### Key Features of AWS Audit Manager

1. **Automated Evidence Collection**: Audit Manager automates the collection of evidence related to the use of AWS resources, which helps to ensure that the data gathered is consistent and accurate. This reduces the manual effort needed to prepare for compliance audits.
    
2. **Pre-built Frameworks**: The service provides pre-built frameworks for common industry standards and regulations, such as GDPR, HIPAA, PCI-DSS, and others. These frameworks include specific control mappings that align AWS usage with the compliance requirements of these standards.
    
3. **Custom Frameworks**: Organizations can also create custom frameworks tailored to their specific compliance needs. This allows for flexibility and ensures that all unique aspects of an organization’s compliance requirements are covered.
    
4. **Audit-ready Reports**: Audit Manager organizes the collected evidence and creates comprehensive audit reports that are designed to be shared with auditors. These reports help simplify the audit process by providing clear and organized documentation of compliance.
    
5. **Continuous Monitoring**: It continuously monitors your AWS resource usage to ensure compliance with chosen frameworks. This helps identify and address compliance issues as they arise, rather than only during periodic audits.
    
6. **Integration with AWS Services**: Works seamlessly with other AWS services, such as AWS Config, AWS CloudTrail, and AWS Security Hub, leveraging their capabilities to enhance compliance data collection and management.
    

### How It Works

- **Select or Create a Framework**: You start by choosing a pre-built compliance framework or creating a custom one based on your specific needs. Each framework consists of a set of controls, which are guidelines or rules that need to be followed to achieve compliance.
    
- **Set Up the Audit**: Define the AWS resources that you want to assess, and Audit Manager will map these resources to the controls in the framework you have selected.
    
- **Automated Data Collection**: Audit Manager automatically collects evidence from the defined AWS resources. This evidence could include configuration snapshots, user activity logs, and other relevant data that demonstrate compliance with the controls.
    
- **Review and Manage Evidence**: You can review the collected evidence and add any additional documentation as needed. Audit Manager allows you to annotate and manage the evidence directly within the service.
    
- **Generate Reports**: Once the evidence collection phase is complete, Audit Manager can generate detailed audit reports that document the compliance status of the resources assessed. These reports can be used directly in internal and external audits.
    

### Benefits

- **Efficiency**: Greatly reduces the time and effort required to prepare for audits by automating many of the tasks associated with evidence collection and report generation.
- **Accuracy**: Enhances the accuracy of compliance assessments by using automated processes to collect evidence, reducing the chance of human error.
- **Continuous Compliance**: Helps maintain continuous compliance with regulatory standards by providing ongoing monitoring and reporting of AWS resource usage.

### Use Cases

- **Regulatory Compliance Audits**: Ideal for organizations that need to comply with strict regulatory standards and undergo regular audits, such as financial services, healthcare, and public sector organizations.
- **Internal Compliance Checks**: Useful for performing regular internal audits to ensure that company policies and procedures are being followed correctly in the use of AWS services.
- **Risk Management**: Helps identify and manage risks associated with non-compliance by providing insights into areas where compliance controls may not be fully met.

AWS Audit Manager is a powerful tool for organizations looking to streamline their compliance and audit processes, making it easier to manage the complexities of regulatory and internal audits in the cloud environment.