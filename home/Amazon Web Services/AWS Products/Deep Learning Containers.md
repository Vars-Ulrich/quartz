---
sticker: vault//Media/icons/aws-icons/DeepLearningContainers.svg
---
# Overview

AWS Deep Learning Containers (DLCs) are Docker images pre-installed with deep learning frameworks to make it easier to deploy, maintain, and scale deep learning environments. They provide a highly reliable and efficient way to build, train, and deploy machine learning models on Amazon Web Services.

### Key Features of AWS Deep Learning Containers

1. **Pre-installed Frameworks**: AWS DLCs come with popular deep learning frameworks such as TensorFlow, PyTorch, and MXNet. These frameworks are optimized for high performance on AWS, both on CPUs and GPUs, ensuring efficient training and inference.
    
2. **Support for Multiple Platforms**: AWS Deep Learning Containers are compatible with AWS services that facilitate machine learning workflows, including Amazon EC2, Amazon ECS (Elastic Container Service), Amazon EKS (Elastic Kubernetes Service), and AWS Fargate for serverless deployment.
    
3. **Continuous Updates and Security**: Amazon continuously updates the deep learning containers, providing not just the latest versions of machine learning frameworks but also ensuring that the containers include the latest security patches.
    
4. **Environment Consistency**: Using containers ensures that your deep learning environment is consistent across your local development environments, training environments, and production. This reduces "works on my machine" issues significantly.
    
5. **Scalability and Portability**: Containers can be easily scaled and are portable across different AWS environments, making it easier to move models from development to production without compatibility issues.
    
6. **Ease of Use**: AWS DLCs simplify the setup process. You can pull a Docker image with everything pre-installed and configured, reducing the overhead of setting up and configuring your machine learning environment.
    

### How It Works

- **Select and Pull Container Image**: Choose the right Docker container image for your deep learning framework from the AWS ECR (Elastic Container Registry). Each image is tagged with the framework version and whether it's optimized for CPU or GPU.
    
- **Run the Container**: You can run these containers locally on your machine, in Amazon EC2 instances, or manage them through Amazon ECS or EKS for scalable and managed deployment. These containers can be used directly or customized further depending on your project needs.
    
- **Develop and Train Models**: Within the container, you can develop and train your machine learning models using the pre-installed frameworks. The environment is already optimized for AWS, ensuring you get the best performance out of your compute resources.
    
- **Deploy Models**: Once training is complete, you can easily deploy your models into production using the same container or use AWS services like Amazon SageMaker for deployment and scaling.
    

### Benefits

- **Reduced Configuration Time**: Significantly reduces the time and effort required to configure and maintain machine learning environments, letting you focus more on model development and training.
    
- **Optimized Performance**: Ensures that you are using versions of deep learning frameworks that are optimized for performance on AWS, helping reduce training times and operational costs.
    
- **Improved Collaboration and Consistency**: Helps maintain consistency across the development lifecycle, from research to production, improving collaboration among team members.
    

### Use Cases

- **Machine Learning Research and Development**: Ideal for ML practitioners and researchers who need a consistent and optimized environment for model development and experimentation.
    
- **Production Deployment**: Suitable for deploying and scaling machine learning models in production environments, ensuring high availability and performance.
    
- **Educational Purposes**: Useful in academic settings where students need a quick and easy way to start with machine learning without the hassle of environment setup.
    

AWS Deep Learning Containers provide a robust, scalable, and efficient way to handle machine learning workflows, enabling faster deployment and easier management of deep learning applications across a wide range of AWS services.