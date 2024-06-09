---
icon: AiDetective
aliases:
  - Amazon Detective
---
# Overview

AWS Detective is a service provided by Amazon Web Services designed to help security teams conduct faster and more efficient investigations into security issues across their AWS workloads. Detective automatically collects log data from AWS resources and uses machine learning, statistical analysis, and graph theory to build a linked set of data that enables users to easily conduct deeper analysis and get to the root cause of potential security issues.

### Key Features of AWS Detective

1. **Automated Data Aggregation and Processing**: AWS Detective automatically aggregates and processes data from AWS CloudTrail and Amazon VPC Flow Logs. It organizes this data into a graph model that summarizes resource behaviors and interactions observed across your AWS environment.
    
2. **Easy to Start**: Setting up AWS Detective is straightforward; you simply enable it in your AWS Management Console, and it begins analyzing historical data to provide immediate insights without any need for additional infrastructure or software.
    
3. **Interactive Visualizations**: It provides a graphical interface that visualizes the interactions between resources, making it easier for security analysts to analyze and understand the relationships and behaviors of resources within their AWS environment.
    
4. **Historical Data Analysis**: Detective maintains up to a year of historical data, allowing teams to conduct security analyses over extended periods to identify trends or investigate past incidents.
    
5. **Integration with AWS Security Services**: It integrates well with AWS Security Hub and Amazon GuardDuty, allowing for seamless transitions from alerts in those services to detailed investigations in Detective.
    

### How It Works

- **Data Collection**: AWS Detective automatically collects log data from integrated AWS services such as AWS CloudTrail and Amazon VPC Flow Logs. This data includes information about API calls, network traffic, and more.
    
- **Data Analysis and Graph Creation**: The service processes and analyzes this data using advanced analytical techniques to create a comprehensive graph of relationships and interactions between AWS resources.
    
- **Investigation and Interaction**: Security analysts use the interactive visual interface to explore the graph. They can quickly determine the extent of potentially malicious activity, identify the resources involved, understand the actions performed, and trace the origin of these activities.
    
- **Incident Response**: Insights gained from AWS Detective can be used to adjust security policies, enhance security measures, and take remedial actions to mitigate and prevent future security threats.
    

### Benefits

- **Efficiency in Security Investigations**: Speeds up the investigation time of security incidents by providing clear and detailed visualizations of resource relationships and interactions.
    
- **Depth of Analysis**: Offers deep analytical capabilities that help uncover hidden patterns and trends that might indicate sophisticated and complex security threats.
    
- **Scalability**: Handles large volumes of log data and integrates across many AWS accounts, making it suitable for enterprises with extensive AWS deployments.
    
- **No Upfront Cost or Additional Infrastructure**: As a managed service, AWS Detective does not require any additional hardware or upfront costs, and you pay only for the data ingested and analyzed.
    

### Use Cases

- **Security Incident Investigations**: When unusual activity is detected by AWS GuardDuty or flagged by AWS Security Hub, AWS Detective helps security teams investigate these activities to determine their nature and scope.
    
- **Compliance Audits**: Helps in performing compliance audits by providing detailed information on resource access patterns and changes over time.
    
- **Operational Troubleshooting**: Beyond security, the detailed interaction graphs can help in operational troubleshooting by identifying configuration changes and interactions that could affect system performance.
    

AWS Detective enhances the ability of security teams to perform proactive security and incident response, providing essential tools needed to understand and protect AWS environments effectively.