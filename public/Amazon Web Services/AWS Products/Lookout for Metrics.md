---
sticker: vault//Media/icons/aws-icons/LookoutForMetrics.svg
---
# Overview

AWS Lookout for Metrics is an anomaly detection service provided by Amazon Web Services that uses machine learning (ML) to automatically detect and diagnose anomalies (outliers from normal patterns) in business and operational data. This service is designed to help businesses improve their operational efficiency and reduce potential losses by quickly identifying unexpected changes in metrics.

### Key Features of AWS Lookout for Metrics

1. **Automated Anomaly Detection**: AWS Lookout for Metrics uses machine learning models to automatically identify anomalies in your data without the need to develop custom ML models. It learns the normal patterns of your metrics and flags deviations that could indicate issues.
    
2. **Wide Range of Data Sources**: The service can integrate with a variety of data sources, including Amazon S3, Amazon Redshift, Amazon RDS, Amazon CloudWatch, and third-party sources such as Salesforce, Marketo, Google Analytics, and more.
    
3. **Real-Time and Historical Data Analysis**: It allows for the analysis of both real-time streaming data and historical data, enabling businesses to detect anomalies as they occur and analyze past data for insights.
    
4. **Customizable Alerts**: You can set up customized alerts that trigger notifications via channels like Amazon SNS (Simple Notification Service), allowing relevant stakeholders to take immediate action based on detected anomalies.
    
5. **Root Cause Analysis**: AWS Lookout for Metrics not only detects anomalies but also helps users understand potential causes by highlighting related anomalies and correlating impacted metrics.
    
6. **Low False Positive Rate**: The service is designed to minimize false positives, ensuring that users spend their time addressing genuine issues.
    

### How It Works

- **Connect Data Sources**: Configure AWS Lookout for Metrics to connect to your data sources. This includes setting up permissions and providing the service with access to the data it needs to analyze.
    
- **Select Metrics**: Choose the specific metrics you want to monitor. The service uses these metrics to learn normal behavior patterns and identify deviations.
    
- **Model Training and Tuning**: AWS Lookout for Metrics automatically trains and tunes machine learning models based on the historical data of your chosen metrics. No machine learning expertise is required from the user.
    
- **Anomaly Detection and Alerts**: Once operational, the service continuously monitors data streams for anomalies. When an anomaly is detected, it triggers an alert according to the configurations you've set up.
    
- **Review and Action**: Users review the detected anomalies and alerts in the service dashboard, investigate potential causes, and take appropriate actions based on insights provided by the service.
    

### Benefits

- **Proactive Issue Resolution**: Helps businesses proactively address issues by detecting anomalies early, often before they can have a significant impact.
    
- **Operational Efficiency**: Improves operational efficiency by automating the monitoring of key performance indicators and operational metrics.
    
- **Cost-Effective**: Reduces the cost associated with manual monitoring and the potential losses from undetected issues.
    
- **Easy to Use**: Simplifies the process of setting up and managing anomaly detection with an intuitive interface and automated ML processes.
    

### Use Cases

- **Business Metrics Monitoring**: Monitor business metrics like sales, revenue, and customer engagement to quickly detect and respond to unexpected drops or spikes.
    
- **Operational Performance**: Track operational metrics such as system performance, application latency, and error rates to ensure smooth operations.
    
- **Marketing Campaign Monitoring**: Evaluate the performance of marketing campaigns by detecting anomalies in engagement metrics or campaign ROI.
    
- **Fraud Detection**: Identify potentially fraudulent activities by spotting unusual patterns in transaction data or user behavior metrics.
    

AWS Lookout for Metrics is a valuable tool for any organization that depends on continuous data monitoring to ensure operational stability and efficiency. It leverages advanced machine learning techniques to provide reliable anomaly detection, helping businesses stay ahead of potential issues.