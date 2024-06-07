---
_filters: 
_contexts: 
_sort:
  field: rank
  asc: false
  group: false
color: var(--mk-color-blue)
icon: MiSaaBadge
---
# Overview
This is the slop sheet for all thing's Amazon Certified Solutions Architect - Associate Exam

[[SAA Exam Guide.pdf]]

# Exam Scope

## Technologies and concepts that might appear on the exam

- Compute
- Cost management
- Database
- Disaster Recovery
- High Performance
- Management and governance
- Microservices and component delivery
- Migration and data transfer
- Networking, connectivity, and content delivery
- Resiliency
- Security
- Serverless and event-driven design principles
- Storage


## In-scope AWS services and features

### Analytics:

- [[Athena|Amazon Athena]]
- [[Data Exchange|AWS Data Exchange]]
- [[Data Pipeline|AWS Data Pipeline]]
- [[Elastic MapReduce|Amazon EMR]]
- [[Glue|AWS Glue]]
- [[Kinesis|Amazon Kinesis]]
- [[Lake Formation|AWS Lake Formation]]
- [[Managed Streaming for Apache Kafka|Amazon MSK]]
- [[OpenSearch Service|Amazon OpenSearch Service]]
- [[QuickSight|Amazon QuickSight]]
- [[Redshift|Amazon Redshift]]

### Application Integration

- [[AppFlow]]
- [[AppSync]]
- [[EventBridge]]
- [[MQ]]
- [[Simple Notification Service]]
- [[Simple Queue Service]]
- [[Step Functions]]

### AWS Cost Management

- [[Budgets]]
- [[Cost and Usage Report]]
- [[Cost Explorer]]
- [[Savings Plans]]

### Compute

- [[Batch]]
- [[Elastic Cloud Compute]]
- [[EC2 Auto-Scaling]]
- [[Elastic Beanstalk]]
- [[Outposts family]]
- [[Outposts rack]]
- [[Outposts servers]]
- [[Serverless Application Repository]]
- [[VMware Cloud on AWS]]
- [[Wavelength]]

### Containers

- [[ECS Anywhere]]
- [[EKS Anywhere]]
- [[EKS Distro]]
- [[Elastic Container Registry]]
- [[Elastic Container Service]]
- [[Elastic Kubernetes Service]]

### Database

- [[Aurora]]
	- Aurora Serverless
- [[DocumentDB]]
- [[DynamoDB]]
- [[ElastiCache]]
- [[Keyspaces]]
- [[Neptune]]
- [[Quantum Ledger Database]]
- [[Relational Database Service]]
- [[Redshift]]

### Developer Tools

- [[X-Ray]]

### Front-End Web and Mobile

- [[Amplify]]
- [[API Gateway]]
- [[Device Farm]]
- [[Pinpoint]]

### Machine Learning

- [[Comprehend]]
- [[Forecast]]
- [[Fraud Detector]]
- [[Kendra]]
- [[Lex]]
- [[Polly]]
- [[Rekognition]]
- [[SageMaker]]
- [[Textract]]
- [[Transcribe]]
- [[Translate]]

### Management and Governance

- [[Auto-Scaling]]
- [[CloudFormation]]
- [[CloudTrail]]
- [[CloudWatch]]
- [[Command Line Interface]]
- [[Compute Optimizer]]
- [[Config]]
- [[Control Tower]]
- Health Dashboard
- [[License Manager]]
- [[Managed Grafana]]
- [[Managed Service for Prometheus]]
- [[Management Console]]
- [[Organizations]]
- [[Proton]]
- [[Service Catalog]]
- [[Systems Manager]]
- [[Trusted Advisor]]
- [[Well Architected Tool]]

### Media Services

- [[Elastic Transcoder]]
- [[Kinesis Video Streams]]

### Migration and Transfer

- [[Application Discovery Service]]
- [[Application Migration Service]]
- [[Database Migration Service]]
- [[DataSync]]
- [[Migration Hub]]
- snow family
- [[Transfer Family]]

### Networking and Content Delivery

- [[Client VPN]]
- [[CloudFront]]
- [[Direct Connect]]
- [[Elastic Load Balancing]]
- [[Global Accelerator]]
- [[PrivateLink]]
- [[Route 53]]
- [[Site to Site VPN]]
- [[Transit Gateway]]
- [[Virtual Private Cloud]]

### Security, Identity, and Compliance

- [[Artifact]]
- [[Audit Manager]]
- [[Certificate Manager]]
- [[CloudHSM]]
- [[Cognito]]
- [[Detective]]
- [[Directory Service]]
- [[Firewall Manager]]
- [[GuardDuty]]
- [[IAM Identity Center]] (aws [[Single Sign-On]])
- [[Identity and Access Management]]
- [[Inspector]]
- [[Key Management Service]]
- [[Macie]]
- [[Network Firewall]]
- [[Resource Access Manager]]
- [[Secrets Manager]]
- [[Security Hub]]
- [[Shield]]
- [[Web Application Firewall]]

### Serverless

- [[AppSync]]
- [[Fargate]]
- [[Lambda]]

### Storage

- [[Backup]]
- [[Elastic Block Store]]
- [[Elastic File System]]
- [[FSx]]
	- all types
- [[Simple Storage Service]]
- [[Simple Storage Service Glacier]]
- [[Storage Gateway]]


# Self-Pointers and Fleeting Thoughts
- **fucking pay closer attention to the actual punchline of the question** 
- SSE-S3 keys cant be used to audit trail usage of the keys
	- but SSE-KMS keys can
- Solutions can suffer from DNS cashing issues, especially for mobile users.
	- this causes a delay in traffic redirection
		- consider these things with differentiating between [[CloudFront]] and [[Route 53]]
- the only s3 class Snowball devices can input into for data  

# Areas of Weakness (pink highlights elsewhere)
### pricing of multitiered services
- [[Simple Storage Service|S3]]
- [[Elastic File System|EFS]]
- [[Elastic Block Store]]
### Database differentiation
### LB types and specs
- **The Application Load Balancer (ALB) is best suited for load balancing HTTP and HTTPS** traffic and provides advanced request routing targeted at the delivery of modern application architectures, including microservices and containers. Operating at the individual request level ([[Open Systems Interconnection Model#Layer 7 - Application|Layer 7]]), the Application Load Balancer routes traffic to targets within Amazon Virtual Private Cloud (Amazon VPC) based on the content of the request.
- NLB cant do content-based routing
### Cloudtrail insights
- what the fuck even are they bro?
### Kinesis Data Streams vs Firehose
- what firehose can and cannot write to directly
	- Amazon Kinesis Data Firehose is a fully managed service for delivering real-time streaming data to destinations such as Amazon Simple Storage Service (Amazon S3), Amazon Redshift, Amazon OpenSearch Service, Splunk, and any custom HTTP endpoint or HTTP endpoints owned by supported third-party service providers, including Datadog, Dynatrace, LogicMonitor, MongoDB, New Relic, and Sumo Logic.
	- Firehose **cannot** directly write into a DynamoDB table
### Business Intelligence
- overview of the concept
### Limitations of services and products
- What can and cannot write what to where and vice-versa?
### Transfer Charges for RDS read replicas
- cross-region data replication **DOES** incur xfer charges
	- while it does not when the replication is occurring within the same region
		- This is the case regardless of AZs, even cross-AZ. As long as they are within the same region, there are no charges for the transfer
### [[Virtual Private Cloud|VPC]]
- Shared services VPC
### [[Lambda]]
- lamda authorizer?
### [[Cognito]]
- #### User vs Identity pools
	- User Pools
		- Provides built-in user management and authentication.
		- Allows you to create and manage user directories, and handle sign-up, sign-in, and user profile management.
		- Integrates directly with API Gateway for authorization using JWT tokens.
		- **Built-in user management**: Yes
	- Identity pools
		- Provides temporary AWS credentials for users to access AWS services.
		- Primarily used for federating user identities from external identity providers (like Facebook, Google, etc.) to access AWS resources.
		- Does not handle user management directly; instead, **it complements User Pools** by providing access to AWS resources after authentication.
		- **Built-in user management**: No (complements User Pools for federated access)
### [[Blue-green deployment]]
### [[Aurora]]
- provisioned vs serverless clusters
### [[Key Management Service|KMS]]
- multi-region keys
	- refer to practice test # 2_2 (question 7)
### [[Global Accelerator]]
- can use endpoint weights to determine the proportion of traffic that is directed to endpoints in an **endpoint group**
	- This is the better choice for exam questions dealing in blue/green deployments in which problems with **DNS caching** on devices is a foreseeable issue
		- ie: select this over route 53 weighted routing in this case



%% Begin Waypoint %%
- **Practice Exams**

- **Udemy SAA course**
	- **[[Course Code]]**
		- **api-gateway**
		- **cli**
		- **cloudformation**
		- **ebs**
		- **ec2-fundamentals**
		- **efs**
		- **kinesis**
		- **kms**
		- **route53**
		- **s3**
		- **s3-advanced**
		- **sqs**
		- **ssm**

%% End Waypoint %%

[exam details page](https://aws.amazon.com/certification/certified-solutions-architect-associate/)  
[[SAA Exam Guide.pdf]] 
[SAA Official Practice Question Set](https://explore.skillbuilder.aws/learn/course/external/view/elearning/13266/aws-certified-solutions-architect-associate-official-practice-question-set-saa-c03-english)

[AWS Solutions Portfolio](https://aws.amazon.com/solutions/?nc1=f_cc)
[Architecture Center](https://aws.amazon.com/architecture/?nc1=f_cc)


