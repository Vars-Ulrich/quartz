---
sticker: vault//Media/icons/aws-icons/DeepLearningAMIs.svg
---
# Overview

AWS Deep Learning AMIs (Amazon Machine Images) provide machine learning practitioners and researchers with the infrastructure and tools to accelerate deep learning in the AWS cloud, at any scale. These AMIs are pre-installed with popular deep learning frameworks and are optimized for high performance on Amazon EC2 instances.

### Key Features of AWS Deep Learning AMIs

1. **Pre-installed Frameworks**: AWS Deep Learning AMIs come pre-installed with several popular deep learning frameworks, including TensorFlow, Apache MXNet, PyTorch, Chainer, Keras, and Microsoft Cognitive Toolkit. This allows users to avoid the complexity of manual installations and configurations.
    
2. **Support for Multiple Frameworks**: Users can choose from different versions of AMIs tailored to specific frameworks or opt for the Conda-based AMI that supports multiple frameworks in a single AMI. This flexibility lets users select the tool that best matches their development and training needs.
    
3. **Optimized for Performance**: These AMIs are optimized for high performance on AWS hardware, including instances with GPU acceleration (such as the Amazon EC2 P3 and P4 instances). They include GPU-accelerated libraries such as NVIDIA CUDA, cuDNN, and NCCL to speed up training times.
    
4. **Easy to Start and Scale**: With these AMIs, you can quickly launch an EC2 instance pre-configured with everything needed to start developing and training deep learning models. The AMIs support AWS's elastic infrastructure, allowing you to scale up or down based on your processing needs.
    
5. **No Additional Cost**: AWS Deep Learning AMIs are provided at no additional charge. You only pay for the AWS resources (like EC2 instances and EBS storage) that you use.
    
6. **Regular Updates**: Amazon regularly updates these AMIs to include the latest versions of deep learning frameworks and tools, ensuring that users have access to the latest technology for their machine learning projects.
    

### How It Works

- **Select and Launch AMI**: You select the appropriate Deep Learning AMI based on your preferred framework and region from the AWS EC2 console. After configuring your instance settings (like instance type, storage, and security groups), you launch the instance.
    
- **Access and Develop**: Once the instance is running, you can access it via SSH. The environment is pre-configured with Jupyter notebooks, allowing you to start coding and training models immediately.
    
- **Train Models**: Utilize the computational power of AWS to train deep learning models. Leverage GPUs if your instance type supports them to enhance training speed.
    
- **Deploy or Iterate**: After training, you can either deploy your model directly from the instance or use the trained models to iterate further and refine your solutions.
    

### Use Cases

- **Rapid Prototyping**: Quickly prototype new deep learning models without worrying about setting up and maintaining a complex development environment.
    
- **Large-scale Training**: Train models on large datasets using the computational power of AWS, particularly using GPU instances for faster processing.
    
- **Educational Purposes**: Use in academic settings for teaching and research purposes, providing students and researchers with access to industry-standard tools and environments.
    

AWS Deep Learning AMIs are a critical resource for anyone involved in machine learning and AI development, providing an easy, fast, and cost-effective way to run deep learning workloads on the cloud. Whether you are a beginner looking to experiment or a seasoned researcher conducting complex training, these AMIs can significantly streamline your workflow.