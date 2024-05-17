---
sticker: vault//Media/icons/aws-icons/ElementalMediaPackage.svg
---
# Overview

### Service Overview:

AWS Elemental MediaPackage is a scalable and reliable video origination and packaging service that enables broadcasters, content owners, and OTT (Over-the-Top) providers to securely package and deliver live and on-demand video content to viewers across a wide range of devices and platforms. It simplifies the process of preparing and delivering video streams for delivery, offering features for content protection, playback optimization, and scalability.

### Key Features:

1. **Video Packaging**: MediaPackage packages live and on-demand video streams into formats suitable for delivery to various devices and platforms, including HTTP Live Streaming (HLS), Dynamic Adaptive Streaming over HTTP (DASH), and Microsoft Smooth Streaming (MSS).
2. **Content Protection**: MediaPackage supports content protection features such as encryption, Digital Rights Management (DRM), and Secure Packager and Encoder Key Exchange (SPEKE), ensuring secure delivery of video content and compliance with content licensing and distribution requirements.
3. **Adaptive Bitrate Streaming (ABR)**: MediaPackage enables adaptive bitrate streaming, allowing viewers to receive the best possible video quality based on their available bandwidth and device capabilities, with support for multiple bitrates and resolutions.
4. **Live and VOD Packaging**: MediaPackage supports both live and video-on-demand (VOD) content packaging, enabling organizations to deliver a seamless viewing experience for live events, linear channels, and on-demand libraries.
5. **Scalability and Redundancy**: MediaPackage automatically scales to handle large volumes of video streams and viewer demand, provisioning resources dynamically to ensure smooth and reliable stream delivery, with built-in redundancy and failover capabilities for high availability.
6. **Integration with CDNs**: MediaPackage integrates seamlessly with content delivery networks (CDNs) such as Amazon CloudFront, Akamai, and Limelight, allowing organizations to leverage global edge caching and distribution for efficient content delivery and low-latency streaming.
7. **Origin Shielding**: MediaPackage supports origin shielding, enabling organizations to protect their origin servers from traffic spikes and distributed denial-of-service (DDoS) attacks by routing requests through a shield cache layer close to the origin.
8. **Monitoring and Metrics**: MediaPackage provides real-time monitoring and metrics dashboards, allowing users to track key performance indicators (KPIs) such as stream delivery status, error rates, and viewer engagement metrics for optimization and troubleshooting.
9. **CDN Log Delivery**: MediaPackage offers CDN log delivery capabilities, allowing organizations to collect and analyze access logs for video streams delivered through CDNs, with support for integration with Amazon Kinesis Data Firehose for log ingestion and analysis.
10. **AWS Integration**: MediaPackage integrates seamlessly with other AWS services such as AWS Elemental MediaLive for live video encoding, AWS Elemental MediaStore for origin storage, and AWS Elemental MediaTailor for server-side ad insertion, enabling end-to-end video workflows.

### How It Works:

1. **Configuration**: Users configure MediaPackage channels and endpoints, specifying settings such as input sources, packaging formats, DRM configurations, and CDN integration options.
2. **Stream Ingestion**: MediaPackage ingests live or VOD video streams from upstream sources such as AWS Elemental MediaLive, AWS Elemental MediaConnect, or direct ingest endpoints, preparing them for packaging and delivery.
3. **Packaging and Encryption**: MediaPackage packages incoming video streams into formats suitable for delivery to viewers, applying encryption and DRM protection as needed to secure the content during transmission and playback.
4. **CDN Integration**: MediaPackage integrates with CDN providers such as Amazon CloudFront, configuring distribution settings and edge caching policies to optimize content delivery and reduce latency for end-users.
5. **Stream Delivery**: MediaPackage delivers packaged video streams to end-users through CDN edge locations, leveraging global infrastructure and edge caching to ensure fast and reliable stream delivery with adaptive bitrate streaming and playback optimization.
6. **Monitoring and Analytics**: MediaPackage provides real-time monitoring and analytics dashboards, allowing users to monitor stream delivery status, viewer engagement metrics, and CDN performance indicators for optimization and troubleshooting.

### Benefits:

1. **Scalable Video Delivery**: MediaPackage enables scalable and reliable video delivery for live and on-demand content, with automatic scaling and redundancy to handle large volumes of video streams and viewer demand.
2. **Secure Content Protection**: MediaPackage supports content protection features such as encryption, DRM, and SPEKE integration, ensuring secure delivery of video content and compliance with content licensing and distribution requirements.
3. **Adaptive Bitrate Streaming**: MediaPackage enables adaptive bitrate streaming, allowing viewers to receive the best possible video quality based on their available bandwidth and device capabilities, with support for multiple bitrates and resolutions.
4. **High Availability and Redundancy**: MediaPackage offers built-in redundancy and failover capabilities, ensuring high availability and reliability for stream delivery, with automatic failover and recovery mechanisms to mitigate disruptions and ensure continuous playback.
5. **CDN Integration and Edge Caching**: MediaPackage integrates seamlessly with CDN providers such as Amazon CloudFront, leveraging global edge caching and distribution for efficient content delivery, low-latency streaming, and improved viewer experiences.
6. **Monitoring and Analytics**: MediaPackage provides real-time monitoring and analytics dashboards, allowing users to track key performance metrics, viewer engagement indicators, and CDN performance data for optimization and troubleshooting, with insights into stream delivery status, error rates, and viewer engagement metrics.
7. **Simplified Workflow**: MediaPackage simplifies the video delivery workflow by handling the complexities of video packaging, encryption, and CDN integration, allowing users to focus on content creation and audience engagement without managing infrastructure or deployment.
8. **Cost-Effective Solution**: MediaPackage offers a cost-effective solution for video origination and packaging, with pay-as-you-go pricing and no upfront fees, allowing organizations to scale their video delivery operations without overprovisioning resources or incurring unnecessary costs.
9. **Flexibility and Compatibility**: MediaPackage supports a wide range of input sources, output formats, and DRM solutions, ensuring compatibility with existing video workflows, encoding pipelines, and playback devices for seamless integration and migration.
10. **Global Reach and Scale**: MediaPackage leverages AWS's global infrastructure and network of edge locations to deliver video streams to viewers worldwide, with low-latency streaming, global redundancy, and high availability for optimal viewer experiences.

### Use Cases:

1. **OTT Video Streaming**: MediaPackage powers OTT (Over-the-Top) video streaming services, enabling broadcasters and content providers to package and deliver live and on-demand video content to viewers across multiple devices, including smart TVs, streaming media players, and mobile devices.
2. **Live Event Broadcasting**: MediaPackage facilitates live event broadcasting for sports, concerts, conferences, and other live events, allowing organizers to deliver high-quality video streams to remote viewers with low latency and adaptive bitrate streaming for optimal viewing experiences.
3. **VOD Content Distribution**: MediaPackage supports video-on-demand (VOD) content distribution for movie studios, content aggregators, and streaming platforms, enabling the secure packaging and delivery of premium video content to subscribers and rental customers worldwide.
4. **Enterprise Video Communications**: MediaPackage serves enterprise video communications and corporate training applications, allowing organizations to stream live and on-demand video content to employees, partners, and customers for internal communications, training, and knowledge sharing.
5. **Education and E-Learning**: MediaPackage powers e-learning platforms and educational institutions in delivering live lectures, virtual classrooms, and on-demand course content to students and learners, with support for secure video delivery and scalable streaming infrastructure.
6. **Media and Entertainment**: MediaPackage caters to media and entertainment companies in distributing live sports, news, and entertainment content to global audiences, with features for content protection, ad insertion, and multiscreen delivery across traditional and digital channels.
7. **Government and Public Sector**: MediaPackage supports government agencies and public sector organizations in broadcasting live government proceedings, public meetings, and emergency announcements to citizens and stakeholders, enhancing transparency and civic engagement.
8. **Healthcare Telemedicine**: MediaPackage facilitates healthcare providers in delivering live telemedicine consultations, medical procedures, and remote diagnostics to patients and healthcare professionals, ensuring secure and HIPAA-compliant video delivery for virtual healthcare services.
9. **Retail and E-Commerce**: MediaPackage enables retailers and e-commerce businesses to showcase live product demonstrations, virtual shopping experiences, and interactive marketing campaigns to customers, driving engagement and sales conversions with rich media content delivery.
10. **Digital Media Archives**: MediaPackage assists organizations in digitizing and archiving historical video content, film libraries, and legacy media assets, with support for secure packaging, long-term storage, and preservation of valuable video archives for future generations.

AWS Elemental MediaPackage empowers organizations to securely package and deliver live and on-demand video content to viewers worldwide, with scalable, reliable, and cost-effective video origination and packaging solutions tailored to their specific needs and use cases.
