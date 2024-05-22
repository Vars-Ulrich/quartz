---
icon: AiKinesisVideoStreams
---
# Overview

AWS Kinesis Video Streams is a fully managed AWS service designed to make it easy to securely stream video from connected devices to AWS for analytics, machine learning (ML), and other processing. AWS Kinesis Video Streams is particularly useful for applications requiring real-time and batch video data processing, such as security monitoring, machine learning model training, and other video analytics applications.

### Key Features of AWS Kinesis Video Streams

1. **Secure Video Ingestion**: Kinesis Video Streams provides a secure channel for streaming video from devices over the internet to the AWS cloud. The service handles various video formats and securely and reliably transfers the streams.
    
2. **Real-Time and Batch Video Processing**: Enables both real-time and batch video processing, allowing for immediate analysis and insights, as well as subsequent processing at a later time.
    
3. **Seamless Integration with AWS Services**: Integrates with other AWS services, including Amazon Rekognition Video for video analysis, AWS Lambda for running processing functions, Amazon S3 for video storage, and Amazon SageMaker for building custom machine learning models that operate on video data.
    
4. **Automatic Scaling**: Automatically scales the infrastructure needed to ingest and store video streams, eliminating the need to manage the underlying server infrastructure.
    
5. **Durable Storage**: Provides options to durably store, encrypt, and index video data in the cloud, enabling easy retrieval and archival of video streams.
    
6. **SDKs and APIs**: Offers SDKs and APIs that make it easy to stream video from various devices, be it consumer mobile apps or specialized camera systems used in surveillance.
    

### How It Works

- **Stream Setup**: You create a video stream resource within AWS Kinesis Video Streams through the AWS Management Console or programmatically via the AWS SDK.
    
- **Device Configuration**: Configure your devices (such as cameras or smartphones) to connect to the Kinesis Video Streams endpoint. Devices use standard media protocols like RTSP (Real-Time Streaming Protocol) to push video to the stream.
    
- **Video Ingestion**: Video data is ingested into Kinesis Video Streams, where it is securely stored and encrypted. The data can then be processed in real-time or stored for batch processing later.
    
- **Video Processing and Analysis**: The ingested video can be processed using integrated AWS services. For instance, use Amazon Rekognition Video for facial recognition, object detection, and activity detection directly on the streamed video.
    
- **Data Storage and Retrieval**: Video data can be archived in Amazon S3 for long-term storage and future analysis. Kinesis Video Streams provides indexing and search capabilities to quickly locate relevant video content within the archived data.
    

### Benefits

- **Enhanced Security Monitoring**: Ideal for applications in security and surveillance, where real-time video streaming and analysis are crucial for incident detection and response.
    
- **Healthcare Monitoring**: In healthcare settings, continuous monitoring and analysis of patient video streams can provide critical real-time data to medical professionals.
    
- **Consumer Media Applications**: Facilitates live video features for consumer applications, enhancing user engagement and content value.
    
- **Industrial Monitoring**: Useful in industrial environments for monitoring equipment and processes, helping in preventive maintenance and safety checks.
    

### Use Cases

- **Home Security Systems**: Stream video from home security cameras to the cloud, where it can be analyzed for unusual activity, person detection, or other specific events.
    
- **Traffic Management**: Monitor traffic conditions in real time using video streams to manage traffic flow and detect incidents on roads and highways.
    
- **Live Event Broadcasting**: Stream live events directly to a broad audience over the internet, integrating real-time analytics to enhance viewer engagement.
    

AWS Kinesis Video Streams offers a robust platform for handling live video feeds from millions of devices, providing comprehensive tools to capture, process, and analyze video data in real time and at scale. This service is a cornerstone for developers looking to integrate advanced video analytics into their applications.