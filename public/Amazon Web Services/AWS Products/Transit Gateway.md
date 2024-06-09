---
icon: AiTransitGateway
aliases:
  - AWS Transit Gateway
---
# Transit Gateway
AWS Transit Gateway connects VPCs and on-premises networks through a central hub. This simplifies your network and puts an end to complex peering relationships. It acts as a cloud router – each new connection is only made once. As you expand globally, inter-Region peering connects AWS Transit Gateways using the AWS global network. Your data is automatically encrypted and never travels over the public internet.

### Service Overview:

AWS Transit Gateway is a fully managed service that simplifies network connectivity by acting as a hub that connects multiple virtual private clouds (VPCs), on-premises networks, and AWS Direct Connect gateways, enabling centralized management and routing of traffic across the AWS cloud infrastructure.

### Key Features:

1. **Hub and Spoke Architecture**: AWS Transit Gateway uses a hub and spoke architecture to connect multiple VPCs, on-premises data centers, and remote networks, providing a centralized point of connectivity and management for network traffic.
2. **Centralized Routing**: Transit Gateway simplifies network routing by allowing administrators to define routing policies and route traffic between connected networks using static routes, dynamic routing protocols (BGP), or route tables.
3. **Network Isolation**: Transit Gateway enables network segmentation and isolation by allowing administrators to create separate transit gateways for different network environments or business units, ensuring logical separation of traffic and resources.
4. **Scalability and Performance**: Transit Gateway scales horizontally to support thousands of VPCs and on-premises connections, providing high throughput and low-latency connectivity for network traffic across the AWS cloud infrastructure.
5. **Transitive Routing**: Transit Gateway supports transitive routing, allowing traffic to flow between connected networks without the need for complex peering relationships or overlapping IP address ranges, simplifying network design and management.
6. **Security and Compliance**: Transit Gateway integrates with AWS Identity and Access Management (IAM) and AWS Key Management Service (KMS) to enforce security controls, encryption, and compliance with regulatory requirements for network traffic.
7. **Monitoring and Visibility**: Transit Gateway provides centralized monitoring and visibility into network traffic, bandwidth utilization, and connectivity status through integration with AWS CloudWatch, enabling administrators to monitor and troubleshoot network issues.
8. **Inter-Region Peering**: Transit Gateway supports inter-region peering, allowing organizations to connect VPCs and on-premises networks across different AWS regions, enabling global network connectivity and redundancy.
9. **Integration with Transit Gateway Network Manager**: Transit Gateway integrates with Transit Gateway Network Manager, a centralized management tool that provides a unified view of network resources, topology visualization, and troubleshooting capabilities.
10. **Cost Optimization**: Transit Gateway offers cost-effective pricing based on usage, allowing organizations to pay only for the resources they consume, without upfront costs or long-term commitments, optimizing cost efficiency and resource utilization.

### How It Works:

1. **Deployment**: Administrators deploy a Transit Gateway in their AWS account and configure connections to VPCs, on-premises networks, and Direct Connect gateways using the AWS Management Console, CLI, or API.
2. **Connection Establishment**: Administrators establish connections between the Transit Gateway and connected networks by creating attachments, such as VPC attachments, VPN attachments, or Direct Connect attachments, and associating them with route tables.
3. **Routing Configuration**: Administrators configure routing policies for the Transit Gateway by creating route tables and defining route propagation rules, route priorities, and routing domains to control the flow of traffic between connected networks.
4. **Traffic Flow**: Once configured, Transit Gateway routes traffic between connected networks based on the routing policies and route tables, enabling seamless connectivity and communication between VPCs, on-premises networks, and external resources.
5. **Monitoring and Management**: Administrators monitor and manage the Transit Gateway using the AWS Management Console, CLI, or API, accessing metrics, logs, and configuration settings to optimize network performance and troubleshoot issues as needed.

### Benefits:

1. **Simplified Network Connectivity**: Transit Gateway simplifies network connectivity by providing a centralized hub for connecting multiple VPCs, on-premises networks, and Direct Connect gateways, reducing complexity and administrative overhead.
2. **Scalability and Performance**: Transit Gateway scales horizontally to support thousands of VPCs and on-premises connections, providing high throughput and low-latency connectivity for network traffic across the AWS cloud infrastructure.
3. **Centralized Management**: Transit Gateway offers centralized management and control over network resources, routing policies, and connectivity settings, enabling administrators to streamline network operations and configuration changes.
4. **Cost Optimization**: Transit Gateway offers cost-effective pricing based on usage, allowing organizations to pay only for the resources they consume, without upfront costs or long-term commitments, optimizing cost efficiency and resource utilization.
5. **Transitive Routing**: Transit Gateway supports transitive routing, allowing traffic to flow between connected networks without the need for complex peering relationships or overlapping IP address ranges, simplifying network design and management.
6. **Inter-Region Connectivity**: Transit Gateway supports inter-region peering, enabling organizations to connect VPCs and on-premises networks across different AWS regions, providing global network connectivity and redundancy.
7. **Security and Compliance**: Transit Gateway integrates with AWS security services and compliance tools to enforce security controls, encryption, and compliance with regulatory requirements for network traffic, ensuring data protection and privacy.
8. **Operational Efficiency**: Transit Gateway streamlines network operations and troubleshooting by providing centralized monitoring, visibility, and management tools, enabling administrators to monitor network performance and resolve issues proactively.

### Use Cases:

1. **Multi-VPC Connectivity**: Organizations use Transit Gateway to connect multiple VPCs within the same AWS account or across different AWS accounts, enabling seamless communication and resource sharing between VPCs.
2. **Hybrid Cloud Connectivity**: Enterprises use Transit Gateway to connect their on-premises data centers and branch offices to AWS cloud resources, enabling hybrid cloud architectures for applications and workloads.
3. **Global Network Integration**: Multinational corporations use Transit Gateway to build global networks spanning multiple AWS regions, enabling inter-region connectivity and data replication for business continuity and disaster recovery.
4. **Network Segmentation**: Organizations use Transit Gateway to segment their network environments and applications into logical compartments, providing isolation and security controls for sensitive workloads and data.
5. **Transit VPC**: Service providers and managed service providers (MSPs) use Transit Gateway to implement transit VPC architectures, serving as a central hub for connecting customer VPCs and managing network traffic.
6. **SaaS Connectivity**: Software as a Service (SaaS) providers use Transit Gateway to provide connectivity and integration with customer VPCs, enabling secure and scalable access to SaaS applications and services.

AWS Transit Gateway provides organizations with a scalable, reliable, and cost-effective solution for simplifying network connectivity, enabling seamless communication and integration between VPCs, on-premises networks, and external resources within the AWS cloud infrastructure.