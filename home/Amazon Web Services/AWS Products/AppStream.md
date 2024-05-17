---
sticker: vault//Media/icons/aws-icons/AppStream.svg
aliases:
  - AppStream 2.0
---
# Overview

AWS AppStream 2.0 is a fully managed, secure application streaming service provided by Amazon Web Services. It allows you to stream desktop applications from AWS to any device, running in a web browser or via a native application, without needing to rewrite them. AppStream 2.0 is designed to provide users with instant access to their applications from anywhere, while securely storing data and running applications in AWS.

### Key Features of AWS AppStream 2.0

1. **Fully Managed Service**: AppStream 2.0 is a managed service, which means AWS handles infrastructure, maintenance, scaling, and updates, allowing you to focus on providing your applications to users.
    
2. **Application Streaming**: Users can access applications through their web browser or a native client. The applications run on AWS, and only the application UI is streamed to the user's device, ensuring that the data never leaves the AWS environment.
    
3. **Secure**: Integration with AWS Identity and Access Management (IAM), network isolation using Amazon VPC, and built-in encryption of data at rest and in transit ensure that your application data is secure.
    
4. **Scalable and Elastic**: Automatically scales to adjust to varying numbers of users without any manual intervention. You can stream applications to a few users or tens of thousands worldwide without any changes to your applications.
    
5. **User Environment Customization**: Allows you to customize the user environment, including applications, network settings, and even the instance type used to run streamed applications.
    
6. **Persistent User Storage**: Offers the option for each user to have persistent storage, so that data can be saved between sessions, providing a seamless experience across sessions.
    

### How It Works

- **Set Up Application Image**: You start by creating an image with all the necessary applications installed. This image will be used to stream applications to your users.
- **Launch Instances**: Once the image is ready, you launch streaming instances based on this image. You can select the appropriate instance type based on the computing, memory, and GPU requirements of your applications.
- **User Access**: Users can then access the applications through a web browser or native AppStream 2.0 client. They interact with the application as if it were installed on their local machine, but all processing happens on the AWS cloud.
- **Session Control**: Administrators have control over session settings, including timeout policies and network access.

### Benefits

- **Accessibility**: Provides users with access to the applications they need on any computer, whether they are using Windows, Linux, Mac, or mobile devices, without requiring any local installations.
- **Centralized Management**: Simplifies the management of software updates and application deployments. When an application is updated on the master image, all users get access to the updated version.
- **Cost Efficiency**: You pay only for the streaming hours that you use, and there are no upfront costs or long-term contracts. This can be more cost-effective than managing physical desktops or laptops, especially for a fluctuating workforce.
- **Performance**: Delivers a high-performance user experience, even with graphics-intensive applications, by leveraging GPU instances.

### Use Cases

- **Corporate Access**: Ideal for providing employees secure access to business applications from anywhere, especially in BYOD (Bring Your Own Device) scenarios.
- **Education**: Allows educational institutions to provide students with access to specialized software needed for courses without requiring high-performance hardware on the student’s part.
- **Software Trials and Demos**: Software vendors can use AppStream 2.0 to let potential customers try their software instantly, without complex installations or fear of software piracy.

AWS AppStream 2.0 represents a powerful solution for organizations looking to provide secure, scalable access to desktop applications across a distributed workforce or customer base.

