---
icon: AiDistroForOpenTelemetry
---
# Overview

AWS Distro for OpenTelemetry (ADOT) is a secure, production-ready, AWS-supported distribution of the OpenTelemetry project. OpenTelemetry provides open-source APIs, libraries, and agents to collect distributed traces and metrics for application monitoring. AWS Distro for OpenTelemetry enhances the OpenTelemetry components to offer a seamless monitoring solution that can integrate efficiently with AWS services.

### Key Features of AWS Distro for OpenTelemetry

1. **Seamless Integration with AWS Services**: ADOT is specifically enhanced to integrate with AWS monitoring services such as Amazon CloudWatch, AWS X-Ray, and Amazon Managed Service for Prometheus. This allows users to send telemetry data (traces, metrics, and logs) directly to these services for analysis and monitoring.
    
2. **Enhanced Support for AWS SDKs**: The distro includes auto-instrumentation agents that automatically capture telemetry data from AWS SDKs. This means that applications using AWS SDKs can be monitored without the need for extensive manual instrumentation.
    
3. **Support for Popular Languages and Frameworks**: ADOT supports several programming languages and frameworks, ensuring that it can be used in a variety of application stacks. This includes support for Java, JavaScript, Python, and .NET, among others.
    
4. **Customization and Flexibility**: While ADOT provides out-of-the-box support for AWS services, it remains flexible and customizable, allowing developers to tweak configurations, data collection, and exports to fit their specific needs or to integrate with other backends that support OpenTelemetry.
    
5. **Community-Driven Innovations**: Being based on the OpenTelemetry project, ADOT benefits from the innovations and contributions of the OpenTelemetry community, ensuring it stays up-to-date with the latest developments in telemetry.
    

### How It Works

- **Instrumentation**: Developers add the OpenTelemetry SDK and the AWS Distro agents or libraries to their application. This instrumentation captures telemetry data from the application itself and the interactions with other services.
    
- **Configuration**: Configure the telemetry data to be collected according to the needs of the application and specify the backend (such as AWS X-Ray or Amazon CloudWatch) where the data should be sent.
    
- **Data Collection and Export**: The AWS Distro for OpenTelemetry collects traces, metrics, and logs during the application runtime. This data is then exported to the specified AWS services for monitoring and analysis.
    
- **Monitoring and Analysis**: Use AWS monitoring services to view and analyze the telemetry data. This can help in debugging, performance monitoring, and ensuring the reliability of your applications.
    

### Benefits

- **Unified Monitoring**: Provides a unified way to collect and monitor logs, metrics, and traces across your entire application stack, both on AWS and on-premises.
    
- **Reduced Overhead**: Automates much of the data collection and exporting process, reducing the manual overhead required to implement effective monitoring.
    
- **Scalability**: ADOT is designed to scale with your applications, handling large volumes of telemetry data without significant overhead.
    
- **AWS Integration**: Leverages deep integrations with AWS services, making it easier for AWS customers to implement observability best practices.
    

### Use Cases

- **Application Performance Monitoring (APM)**: Gain insights into application performance and quickly pinpoint issues with detailed traces and metrics.
    
- **Infrastructure Monitoring**: Monitor the performance and health of infrastructure components using collected metrics and logs.
    
- **Distributed Tracing**: Improve debugging and performance analysis in microservices architectures with distributed tracing that visualizes the entire request path across services.
    

AWS Distro for OpenTelemetry provides a robust solution for AWS customers looking to implement advanced telemetry and monitoring capabilities in their applications, leveraging the open-source power of OpenTelemetry along with the native integration and support of AWS.