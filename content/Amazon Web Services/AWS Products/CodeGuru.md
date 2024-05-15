---
sticker: vault//Media/icons/aws-icons/CodeGuru.svg
---
# Overview

AWS CodeGuru is an innovative service offered by Amazon Web Services that provides automated code reviews and application performance recommendations. It uses machine learning models trained on decades of Amazon's own code reviews and application profiling data to provide insights that help developers optimize their applications and improve code quality. CodeGuru is split into two main components: CodeGuru Reviewer and CodeGuru Profiler.

### Key Features of AWS CodeGuru

#### CodeGuru Reviewer

1. **Automated Code Reviews**: CodeGuru Reviewer scans your code (primarily supports Java and Python) and provides automatic suggestions for improving quality and reducing issues. It detects common coding errors, identifies critical issues, and suggests how to remediate them.
    
2. **Integration with Development Tools**: It integrates seamlessly with existing development workflows and source control systems like GitHub, Bitbucket, and AWS CodeCommit, making it easy to add to your software development lifecycle without disruption.
    
3. **Security Analysis**: CodeGuru Reviewer includes a security analysis feature, which scans your code for security vulnerabilities and provides recommendations on how to fix them. This helps improve the security posture of your applications.
    

#### CodeGuru Profiler

1. **Application Performance Insights**: CodeGuru Profiler helps developers understand the runtime behavior of their applications, identify performance bottlenecks, and get specific recommendations on how to fix them to reduce CPU usage, improve throughput, and reduce latency.
    
2. **Cost Optimization**: By optimizing application performance, CodeGuru Profiler can help reduce the cost of running applications on AWS. It provides insights that can lead to more efficient resource utilization, directly impacting cloud costs.
    
3. **Easy to Use**: The profiler can be used with just a few clicks in the AWS Management Console, and it requires minimal changes to your existing application code to get started.
    

### How It Works

- **CodeGuru Reviewer**: You connect your source code repository to AWS CodeGuru Reviewer. Once integrated, it automatically reviews pull requests made to the repository and comments on optimization opportunities and critical issues directly in the pull request.
    
- **CodeGuru Profiler**: You integrate a small agent into your application, which collects profiling data while the application runs in production or during performance testing. This data is sent to CodeGuru Profiler, which analyzes it and provides visualizations and recommendations through the AWS console.
    

### Benefits

- **Improved Code Quality**: Automatically identifies critical issues, security vulnerabilities, and inefficiencies in code, leading to improved overall code quality.
    
- **Increased Application Performance**: Helps developers optimize their applications by providing actionable insights on how to improve performance and reduce resource consumption.
    
- **Reduced Operational Costs**: Optimizing code and application performance can lead to significant reductions in operational costs, especially in cloud environments where resources are paid for based on usage.
    
- **Enhanced Developer Productivity**: By automating code reviews and performance recommendations, CodeGuru allows developers to focus more on feature development rather than troubleshooting and optimization.
    

### Use Cases

- **Continuous Integration/Continuous Deployment (CI/CD) Pipelines**: Integrating CodeGuru in CI/CD pipelines to ensure code quality and performance standards are met before deployment.
    
- **Performance Optimization**: Using CodeGuru Profiler in development and production environments to continuously monitor and optimize application performance.
    
- **Security Assurance**: Employing CodeGuru Reviewer to enhance the security of applications by detecting and fixing security vulnerabilities early in the development process.
    

AWS CodeGuru is a powerful tool for any organization looking to leverage machine learning to enhance their code quality and application performance, making it an essential part of modern, efficient, and secure software development processes.