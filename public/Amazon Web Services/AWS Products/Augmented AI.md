---
icon: AiAugmentedAIA2I
aliases:
  - A2I
---
# Overview

AWS Augmented AI (Amazon A2I) is a service designed by Amazon Web Services to integrate human reviews into machine learning workflows. This service facilitates the use of human judgment to review machine learning predictions, which is particularly useful in situations where it's necessary to ensure the accuracy of machine learning models or when dealing with subjective decisions that AI alone might not handle effectively.

### Key Features of AWS Augmented AI

1. **Easy Integration with ML Services**: Amazon A2I can be easily integrated with other AWS machine learning services such as Amazon SageMaker (for custom models), Amazon Rekognition, and Amazon Textract. This allows developers to add human review seamlessly where the AI model's confidence is below a certain threshold or in critical decision-making scenarios.
    
2. **Built-in Human Review Workflows**: Amazon A2I provides built-in human review workflows, which can be used directly in applications requiring human oversight. For example, in content moderation, document processing, or any other task that requires validation of machine-generated outputs.
    
3. **Flexibility in Human Review**: Businesses can choose to use Amazon Mechanical Turk, third-party vendors that they have a relationship with, or even their own in-house teams for the human review tasks. This flexibility allows organizations to maintain control over who reviews sensitive or confidential data.
    
4. **Manageable and Scalable**: The service is designed to handle the management and scaling of human review tasks, enabling organizations to review large volumes of predictions without significant increases in operational complexity.
    
5. **Consistency and Quality Control**: Provides tools and settings to help maintain consistency and quality in human reviews, such as providing workers with specific instructions or criteria for review tasks.
    

### How It Works

- **Define a Human Review Workflow**: You start by defining a workflow for human review within Amazon A2I, specifying when and how to send machine learning predictions to human reviewers. This includes setting conditions based on the confidence score of AI predictions.
    
- **Choose Your Workforce**: Select who will perform the reviews—Amazon Mechanical Turk workers, specific vendors, or an internal workforce.
    
- **Integrate with ML Models**: Connect Amazon A2I with your machine learning models, such as those built on Amazon SageMaker, Amazon Rekognition, or Amazon Textract. The integration involves specifying where low-confidence predictions (or other specified conditions) are routed to human reviewers.
    
- **Review and Feedback Loop**: Human reviewers check the AI's work and make the necessary corrections or verifications. The outcomes can be fed back into the machine learning model, creating a feedback loop that improves AI accuracy over time.
    

### Benefits

- **Improves Model Accuracy**: By incorporating human judgment into ML workflows, businesses can greatly improve the accuracy of their models, especially in complex or subjective areas.
- **Reduces Risk**: Helps mitigate risks associated with fully automated decisions, particularly in sensitive areas such as medical diagnoses, financial decisions, or content moderation.
- **Scalability**: Manages the scalability of human reviews as the volume of predictions increases, without corresponding increases in administrative overhead.

### Use Cases

- **Content Moderation**: Human reviewers can assess user-generated content that AI tools flag as potentially offensive or out of policy, ensuring only appropriate content is posted.
- **Financial Services**: In loan applications or insurance claim processing, humans can review cases where the AI model's decision is uncertain, adding an extra layer of scrutiny.
- **Healthcare**: For medical imaging analysis, human experts can review cases flagged by AI for further examination, ensuring high accuracy in diagnoses.

AWS Augmented AI is an essential tool for businesses looking to blend human expertise with the efficiency of machine learning, providing a balanced approach to automated decision-making processes.