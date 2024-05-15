---
sticker: vault//Media/icons/aws-icons/AppMesh.svg
---
# Overview
  
AWS App Mesh is a service mesh that provides application-level networking to make it easy for your services to communicate with each other across multiple types of compute infrastructure. App Mesh standardizes how your services communicate, giving you end-to-end visibility and helping to ensure high-availability for your applications.

### Key Features of App Mesh

1. **Service Discovery Integration**: App Mesh integrates with existing service discovery mechanisms AWS provides, such as Amazon ECS service discovery, Amazon EKS service discovery, and Kubernetes DNS. This integration helps maintain a consistent view of your services.
    
2. **Fine-Grained Traffic Control**: It offers fine-grained traffic routing controls, allowing you to easily route traffic between different versions of services for canary deployments, blue/green deployments, and more.
    
3. **Resiliency**: Implements retries, failover, and circuit breaker capabilities, which enhance the resilience of your service communications.
    
4. **Security**: Supports strong identity and encryption standards using TLS to encrypt communication between your services, thus enhancing security, particularly in a multi-tenant environment.
    
5. **Observability**: Provides out-of-the-box observability features for monitoring and tracing the requests that travel through your mesh. This includes integration with AWS X-Ray for tracing.
    
6. **Protocol Support**: App Mesh supports HTTP, HTTP/2, gRPC, and TCP traffic, which covers a broad set of application types.
    

### How It Works

- **Components**: The primary components of App Mesh are virtual nodes, virtual routers, virtual services, and routes. A virtual node acts as a logical pointer to a particular task group, such as an ECS service or a Kubernetes deployment. Virtual routers handle the traffic between different versions of a service, and routes define how traffic is directed between services.
- **Envoy**: App Mesh uses Envoy, an open-source edge and service proxy, as the primary data plane that manages the network traffic between services. Each instance of your services in the mesh has an Envoy proxy that handles incoming and outgoing service traffic.

### Integration with AWS Services

- **[[Elastic Container Service|ECS]] (Elastic Container Service)**: You can define an App Mesh virtual node as an ECS service, which allows the ECS services to be part of the mesh.
- **[[Elastic Kubernetes Service|EKS]](Elastic Kubernetes Service)** and Kubernetes on EC2: App Mesh is deeply integrated with EKS, allowing Kubernetes services to be part of the mesh. It also works with Kubernetes running on EC2 instances.
- **[[Fargate]]**: AWS Fargate, the serverless compute engine for containers, can also be integrated with App Mesh, enabling you to run serverless mesh services.

### Benefits

- **Application Resilience**: By handling retries, failover, and other network issues transparently, App Mesh increases the overall resilience of your applications.
- **Service Level Insights**: Gain detailed insights into the dependencies between services along with their performance metrics.
- **Security**: Improved security model for your internal service communications with encryption and strong identity enforcement.

### Use Cases

- **Microservices Communication**: App Mesh is ideal for managing complex microservices architectures where services need to communicate securely and reliably.
- **Service Migration**: Helps in gradually migrating services to new versions or configurations without causing downtime or affecting the user experience.
- **Application Scaling**: Supports dynamic scaling of services without the need to reconfigure routing rules manually.

AWS App Mesh is particularly useful for developers and enterprises that are looking to simplify service-to-service communication in their cloud-native applications, providing them with the tools needed to manage, secure, and monitor inter-service interactions effectively.