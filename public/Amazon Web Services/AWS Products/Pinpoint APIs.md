---
icon: AiPinpointAPIs
---
# Overview

AWS Pinpoint provides a set of APIs that enable developers to integrate and interact with the Pinpoint service programmatically. These APIs allow you to manage and automate various aspects of your customer engagement campaigns, including sending targeted messages, tracking user interactions, and analyzing campaign performance. Here's an overview of the key APIs provided by AWS Pinpoint:

### 1. RESTful API:

- **Overview**: The AWS Pinpoint RESTful API allows you to programmatically manage resources such as applications, campaigns, segments, endpoints, and events.
- **Capabilities**: With the REST API, you can create and update campaigns, send messages, manage user segments, register endpoints (e.g., mobile devices, email addresses), and track user events.
- **Authentication**: Authentication for the REST API is handled using AWS Identity and Access Management (IAM) credentials. You need to create IAM users or roles with appropriate permissions to access the Pinpoint API.

### 2. AWS SDKs:

- **Overview**: AWS provides SDKs (Software Development Kits) for various programming languages, including JavaScript, Java, Python, .NET, and others. These SDKs wrap the Pinpoint API, making it easier to integrate Pinpoint functionality into your applications.
- **Capabilities**: The SDKs provide higher-level abstractions and utility functions for interacting with Pinpoint, reducing the amount of boilerplate code you need to write. They handle tasks such as authentication, request signing, and error handling.
- **Usage**: You can use the SDKs to send messages, track events, create and manage campaigns, and perform other Pinpoint operations from within your applications.

### 3. AWS CLI:

- **Overview**: The AWS Command Line Interface (CLI) provides a command-line interface for interacting with various AWS services, including Pinpoint. You can use the CLI to perform common Pinpoint operations from your terminal or shell scripts.
- **Capabilities**: The AWS CLI allows you to manage Pinpoint applications, campaigns, segments, endpoints, and events using simple command-line commands. It provides a convenient way to automate routine tasks and integrate Pinpoint with other command-line tools and scripts.
- **Installation**: You can install the AWS CLI on your local machine or on an Amazon EC2 instance by following the installation instructions provided in the AWS documentation.

### 4. AWS Mobile SDK:

- **Overview**: The AWS Mobile SDKs provide libraries and tools for building mobile applications that interact with AWS services, including Pinpoint. The SDKs support platforms such as iOS, Android, and Unity.
- **Capabilities**: The Mobile SDKs include features for registering endpoints, sending targeted messages, tracking user interactions, and analyzing campaign performance within mobile apps.
- **Integration**: You can integrate the Mobile SDKs into your mobile applications to leverage Pinpoint's capabilities for customer engagement and analytics.

### 5. Event Stream API:

- **Overview**: The Event Stream API allows you to send event data to Pinpoint in real-time using HTTP POST requests. This API is particularly useful for streaming event data from IoT devices, servers, and other sources directly to Pinpoint for analysis and tracking.
- **Usage**: You can use the Event Stream API to track custom events, user interactions, device telemetry, and other types of data that you want to analyze or act upon within Pinpoint.
- **Integration**: You can integrate the Event Stream API into your applications, devices, or backend systems to send event data to Pinpoint using HTTP POST requests.

These are the main APIs provided by AWS Pinpoint for integrating and interacting with the service. They enable you to leverage Pinpoint's capabilities for targeted messaging, user engagement, and campaign analytics in a programmatic and automated manner.