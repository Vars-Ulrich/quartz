---
sticker: vault//Media/icons/aws-icons/SageMakerGroundTruth.svg
---
# Overview

### Service Overview:

Amazon SageMaker Ground Truth is a fully managed data labeling service that makes it easy to build high-quality labeled datasets for machine learning (ML) applications. It helps you efficiently label large volumes of data by providing labeling workflows, annotation tools, and human labelers, allowing you to focus on training and improving ML models instead of managing the labeling process.

### Key Features:

1. **Custom Labeling Workflows**: Ground Truth allows you to create custom labeling workflows tailored to your specific data labeling requirements, including image classification, object detection, text classification, and semantic segmentation.
2. **Automated Labeling**: Ground Truth offers automated labeling capabilities using machine learning algorithms, enabling you to accelerate the labeling process and reduce manual effort.
3. **Human Labeling**: Ground Truth provides access to a global workforce of human labelers who can annotate data with high accuracy and quality, ensuring the reliability of labeled datasets.
4. **Labeling Tooling**: Ground Truth includes built-in annotation tools for various data types, including images, text, and audio, making it easy to annotate data using bounding boxes, polygons, semantic labels, and more.
5. **Active Learning**: Ground Truth supports active learning workflows, allowing you to iteratively improve model performance by identifying and labeling the most informative data points for training.
6. **Quality Control**: Ground Truth provides built-in quality control mechanisms such as consensus labeling and worker qualification, ensuring the accuracy and consistency of labeled datasets.
7. **Integration with SageMaker**: Ground Truth seamlessly integrates with Amazon SageMaker, allowing you to use labeled datasets directly for model training and evaluation within the SageMaker environment.

### How It Works:

1. **Dataset Preparation**: You prepare your raw data by uploading it to Amazon S3 or connecting to other data sources supported by SageMaker Ground Truth.
2. **Labeling Workflow Creation**: You define a custom labeling workflow in Ground Truth, specifying labeling instructions, annotation tasks, and quality control mechanisms.
3. **Labeling Task Assignment**: Ground Truth automatically assigns labeling tasks to human labelers or machine learning algorithms based on your workflow configuration.
4. **Data Annotation**: Human labelers or machine learning algorithms annotate data according to the specified instructions using the built-in annotation tools provided by Ground Truth.
5. **Quality Assurance**: Ground Truth performs quality assurance checks such as consensus labeling and worker qualification to ensure the accuracy and consistency of labeled datasets.
6. **Dataset Delivery**: Once labeled, the datasets are delivered to your Amazon S3 bucket or integrated directly with SageMaker for model training and evaluation.

### Benefits:

1. **High-Quality Labeled Datasets**: Ground Truth helps you generate high-quality labeled datasets quickly and efficiently, enabling better model performance and accuracy.
2. **Time and Cost Savings**: Ground Truth automates and streamlines the data labeling process, saving time and reducing the cost associated with manual labeling efforts.
3. **Scalability**: Ground Truth scales seamlessly to handle large volumes of data labeling tasks, allowing you to label datasets of any size with ease.
4. **Flexibility**: Ground Truth offers flexibility in labeling workflows, annotation tools, and quality control mechanisms, allowing you to tailor the labeling process to your specific requirements.
5. **Integration with SageMaker**: Ground Truth integrates seamlessly with Amazon SageMaker, providing a streamlined workflow for using labeled datasets directly for model training and evaluation.
6. **Consistency and Reliability**: Ground Truth ensures the consistency and reliability of labeled datasets through quality control mechanisms and human labelers with high accuracy and quality standards.

### Use Cases:

1. **Computer Vision**: Use Ground Truth to label images for tasks such as object detection, image classification, facial recognition, and autonomous driving.
2. **Natural Language Processing (NLP)**: Use Ground Truth to annotate text data for tasks such as sentiment analysis, named entity recognition, text classification, and language translation.
3. **Speech Recognition**: Use Ground Truth to transcribe audio data and annotate speech segments for tasks such as speech recognition, speaker identification, and voice-controlled applications.
4. **Medical Imaging**: Use Ground Truth to label medical images for tasks such as disease diagnosis, tumor detection, and medical image segmentation in healthcare applications.
5. **Autonomous Vehicles**: Use Ground Truth to label sensor data from LiDAR, radar, and cameras for tasks such as object detection, lane detection, and obstacle avoidance in autonomous vehicle systems.

Amazon SageMaker Ground Truth simplifies the process of creating high-quality labeled datasets for machine learning applications, allowing you to focus on training and improving ML models without worrying about the complexities of data labeling.