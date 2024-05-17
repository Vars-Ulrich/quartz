---
sticker: vault//Media/icons/aws-icons/CodePipeline.svg
---
# Overview
AWS CodePipeline is a continuous delivery service that enables you to model, visualize, and automate the steps required to release your software. With AWS CodePipeline, you model the full release process for building your code, deploying to pre-production environments, testing your application and releasing it to
production.

AWS CodePipeline integrates with AWS services such as  [[CodeCommit]], [[Simple Storage Service|S3]] [[CodeBuild]], [[CodeDeploy]], [[Elastic Beanstalk]], [[CloudFormation]], [[OpsWorks]], [[Elastic Container Service|ECS]], and [[Lambda]]. To further elucidate, CodePipeline cannot by itself deploy the code, it can integrate with CodeDeploy for the actual deployment.

### Service Overview:

AWS CodePipeline is a fully managed continuous integration and continuous delivery (CI/CD) service that automates the build, test, and deployment phases of releasing software. It enables teams to orchestrate and automate the release process for their applications, allowing for rapid and reliable software delivery.

### Key Features:

1. **Pipeline Orchestration**: CodePipeline allows users to create custom pipelines to model their software release process. Pipelines consist of stages, each containing one or more actions that represent a step in the release process.
2. **Integration with AWS Services**: CodePipeline integrates seamlessly with other AWS services such as AWS CodeBuild, AWS CodeDeploy, AWS Lambda, and third-party tools like Jenkins, enabling end-to-end automation of the software delivery process.
3. **Flexible Workflow**: Users can define custom workflows with multiple stages and actions, enabling them to build, test, and deploy their applications according to their specific requirements.
4. **Visual Pipeline Editor**: CodePipeline provides a visual editor that allows users to create and edit pipelines visually, making it easy to visualize and manage the release process.
5. **Artifact Management**: CodePipeline manages the flow of artifacts (e.g., source code, binaries) through the pipeline, ensuring that the right artifacts are passed between stages and actions.
6. **Triggering and Scheduling**: Pipelines can be triggered automatically by events such as code commits, AWS CloudWatch events, or manually triggered on-demand. Users can also schedule pipeline executions at specific times.
7. **Parallel and Sequential Execution**: Actions within a stage can be executed in parallel or sequentially, allowing users to optimize the release process for performance and reliability.
8. **Approval Gates**: CodePipeline supports manual approval actions that require human intervention before proceeding to the next stage, enabling users to implement governance and compliance checks.
9. **Versioning and History**: CodePipeline maintains a history of pipeline executions, including the version of the artifacts used in each execution, providing visibility and auditability of the release process.
10. **Integration with Third-party Tools**: CodePipeline integrates with popular third-party tools and services through custom actions, allowing users to extend the capabilities of their pipelines and integrate with existing tools and workflows.

### How It Works:

1. **Pipeline Creation**: Users define the stages and actions that make up their release process using the CodePipeline console or API.
2. **Source Stage**: CodePipeline retrieves the source code from a version control system such as AWS CodeCommit, GitHub, or Amazon S3.
3. **Build Stage**: CodePipeline triggers a build process using AWS CodeBuild or a third-party build tool to compile, package, and test the application code.
4. **Test Stage**: CodePipeline executes automated tests using testing frameworks or services to validate the application's functionality and quality.
5. **Deploy Stage**: CodePipeline deploys the application to the target environment using AWS CodeDeploy, AWS Elastic Beanstalk, AWS Lambda, or other deployment services.
6. **Approval Stage**: If manual approval is required, CodePipeline waits for human intervention to approve or reject the deployment before proceeding to the next stage.
7. **Monitor Stage**: CodePipeline monitors the deployment for errors or issues, automatically rolling back the deployment if necessary.
8. **Notification**: CodePipeline sends notifications to stakeholders via Amazon SNS or other notification services, informing them of the pipeline status and deployment outcome.

### Benefits:

1. **Automation**: CodePipeline automates the software release process, reducing manual effort and human errors associated with manual deployments.
2. **Consistency**: CodePipeline ensures consistent and repeatable deployments across different environments, reducing the risk of configuration drift and deployment failures.
3. **Speed**: CodePipeline enables rapid and reliable software delivery, allowing teams to release updates to applications quickly and efficiently.
4. **Flexibility**: CodePipeline offers flexible workflows and integration options, allowing users to tailor the release process to their specific needs and requirements.
5. **Visibility**: CodePipeline provides visibility into the release process with detailed execution logs, versioning, and history, enabling users to track the progress of deployments and troubleshoot issues.
6. **Scalability**: CodePipeline scales automatically to handle deployments of any size and complexity, ensuring reliable performance and availability.

### Use Cases:

1. **Continuous Integration and Delivery**: CodePipeline is used to automate the build, test, and deployment process for web applications, mobile apps, microservices, and other software projects.
2. **Release Management**: CodePipeline facilitates the management of software releases, allowing teams to orchestrate the release process from code commit to deployment in a consistent and reliable manner.
3. **Multi-environment Deployments**: CodePipeline supports multi-environment deployments, enabling teams to deploy applications to development, testing, staging, and production environments with ease.
4. **Infrastructure as Code (IaC)**: CodePipeline is used to automate the deployment of infrastructure changes using tools such as AWS CloudFormation, Terraform, or Ansible, enabling infrastructure updates to be treated as code.
5. **Blue/Green Deployments**: CodePipeline supports blue/green deployments, allowing teams to deploy new application versions alongside existing versions and switch traffic gradually to the new version to minimize downtime and risk.

AWS CodePipeline simplifies and automates the software release process, enabling teams to deliver high-quality software faster and more efficiently.