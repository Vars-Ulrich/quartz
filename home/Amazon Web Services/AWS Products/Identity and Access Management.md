---
sticker: vault//Media/icons/aws-icons/IdentityAndAccessManagement.svg
aliases:
  - IAM
---

# Identity and Access Management

- Global in scale

- Policies written as JSON docs
	- JSON policy doc includes these elements:
		- optional policy-wide information at the top of the doc
		- One or more individual statements
- Two mandatory elements
	- Effect
		- "Allow" or "Deny"
	- Action
		- List of actions that the policy allows/denies
- Four Optional elements
	- Statement ID (Sid)
		- Include an optional statement ID to differentiate between your statements.
	- Principal
		- required only in some circumstances
		- If you create a resource-based policy, you must indicate the account, user, role, or federated user to which you would like to allow or deny access. If you are creating an IAM permissions policy to attach to a user or role, you cannot include this element. The principal is implied as that user or role.
	- Resource
		- If you create an IAM permissions policy, you must specify a list of resources to which the actions apply. If you create a resource-based policy, this element is optional. If you do not include this element, then the resource to which the action applies is the resource to which the policy is attached.
	- Condition
		- Specify circumstances under which policy grants permission

# IAM credentials report
You can generate and download a credential report that lists all users in your account and the status of their various credentials, including passwords, access keys, and MFA devices. It is not used to review permissions granted to a user.

# IAM access advisor
Access advisor shows the service permissions granted to a user and when those services were last accessed. You can use this information to revise your policies. To summarize, you can identify unnecessary permissions so that you can revise your IAM policies accordingly.


[[SAA Course Slides.pdf#page=25&selection=0,0,0,1|SAA Course Slides, page 25]]

### Service Overview:

AWS Identity and Access Management (IAM) is a web service provided by Amazon Web Services (AWS) that enables organizations to securely control access to AWS resources. IAM allows administrators to manage user identities, permissions, and access policies, ensuring that only authorized users and services can interact with AWS resources.

### Key Features:

1. **User Management**: IAM enables administrators to create and manage IAM users, groups, and roles, allowing them to assign unique identities to individuals and services accessing AWS resources.
2. **Access Control Policies**: Administrators can define IAM policies specifying permissions for accessing AWS resources and actions, granting or denying users' requests based on their assigned roles and responsibilities.
3. **Role-Based Access Control (RBAC)**: IAM supports RBAC principles, allowing administrators to assign permissions to roles rather than individual users, simplifying access management and enforcing least privilege principles.
4. **Identity Federation**: IAM supports identity federation with external identity providers (IdPs) such as Microsoft Active Directory, enabling users to authenticate using their existing corporate credentials, reducing the need for separate IAM accounts.
5. **Multi-Factor Authentication (MFA)**: IAM offers MFA capabilities, allowing administrators to add an extra layer of security to user authentication by requiring users to provide additional authentication factors such as SMS codes or hardware tokens.
6. **Access Logging and Monitoring**: IAM provides access logging and monitoring features, allowing administrators to audit IAM activities, review access logs, and analyze security events to detect and respond to unauthorized access attempts.
7. **AWS Organizations Integration**: IAM integrates with AWS Organizations to enable centralized access management across multiple AWS accounts, allowing administrators to enforce access policies and standards consistently.
8. **Identity Policies**: Administrators can create custom identity policies specifying rules and conditions for user authentication, authorization, and access control, tailored to organizational requirements and security policies.

### How It Works:

1. **User Provisioning**: Administrators use IAM to create IAM users, groups, and roles, assigning appropriate permissions and access levels based on users' job roles and responsibilities.
2. **Permission Assignment**: Administrators define IAM policies specifying permissions for accessing AWS resources and actions, using the policy management interface in IAM, and attach these policies to users, groups, or roles.
3. **Access Control Enforcement**: IAM enforces access controls based on IAM policies, allowing or denying users' requests to access AWS resources and perform actions within those resources, according to their assigned permissions.
4. **Authentication and Authorization**: IAM authenticates users' identities when they attempt to access AWS resources, verifying their credentials and determining their assigned permissions and access levels based on IAM policies.
5. **Identity Federation**: IAM supports identity federation with external IdPs, allowing users to authenticate using their existing corporate credentials, federating identities across AWS and on-premises environments.
6. **Access Logging and Monitoring**: IAM logs access events, API calls, and authentication attempts to AWS CloudTrail, allowing administrators to monitor IAM activities, review access logs, and investigate security incidents.
7. **Integration with AWS Services**: IAM integrates seamlessly with other AWS services such as AWS SSO, AWS Organizations, AWS CloudTrail, and AWS Config, providing a unified IAM experience and leveraging the capabilities of the AWS cloud platform for access management and security.

### Benefits:

1. **Improved Security**: IAM helps organizations improve security by enforcing least privilege principles, controlling access to AWS resources, and monitoring access activities to detect and respond to unauthorized access attempts.
2. **Simplified Access Management**: The service simplifies access management by offering a unified interface and tools for defining, enforcing, and monitoring access controls, reducing the complexity of managing IAM policies and permissions.
3. **Scalability and Flexibility**: IAM scales seamlessly to accommodate growing numbers of users, groups, and roles, and adapts to changing business requirements and security needs, providing flexibility and agility for managing IAM resources.
4. **Cost Efficiency**: IAM helps reduce operational costs associated with access management by automating administrative tasks, optimizing access controls, and leveraging the scalability and reliability of the AWS cloud platform.
5. **Compliance and Governance**: IAM enables organizations to achieve compliance with regulatory requirements such as GDPR, HIPAA, PCI DSS, and SOC 2 by enforcing access controls, monitoring access activities, and generating audit reports.

### Use Cases:

1. **Enterprise Identity Management**: Organizations use IAM to manage user identities and access controls across their AWS accounts and services, ensuring consistent security policies and compliance requirements.
2. **Regulatory Compliance**: IAM helps organizations achieve compliance with industry regulations by enforcing access controls, monitoring access activities, and generating audit reports to demonstrate compliance with regulatory requirements.
3. **Cross-Account Access**: Organizations with multiple AWS accounts use IAM to manage cross-account access and permissions, enabling users to access resources in different accounts while maintaining centralized visibility and control.
4. **Identity Federation**: Organizations federate identities with external IdPs using IAM, allowing users to authenticate using their existing corporate credentials, reducing the need for separate IAM accounts and passwords.
5. **Partner and Vendor Access**: Organizations collaborate with external partners and vendors by granting temporary access to AWS resources using IAM, enforcing fine-grained access controls and monitoring access activities for security and compliance purposes.

AWS Identity and Access Management (IAM) empowers organizations to manage user identities, permissions, and access controls effectively, ensuring secure and compliant access to AWS resources and applications. With its robust features, integration capabilities, and scalability, IAM helps organizations streamline access management, strengthen security posture, and drive digital transformation initiatives in the cloud.

