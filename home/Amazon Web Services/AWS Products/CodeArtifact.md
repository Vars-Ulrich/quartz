---
sticker: vault//Media/icons/aws-icons/CodeArtifact.svg
---
# Overview

AWS CodeArtifact is a fully managed artifact repository service provided by Amazon Web Services. It makes it easy for organizations to securely store, publish, and share software packages used in their software development process. CodeArtifact works with commonly used package management tools such as Maven, Gradle, npm, yarn, twine, and pip, making it compatible with a wide array of development workflows.

### Key Features of AWS CodeArtifact

1. **Secure Artifact Management**: AWS CodeArtifact allows you to store, manage, and share software development packages securely within your organization or with external entities.
    
2. **Integration with Existing Tools**: It integrates seamlessly with existing development tools and package managers, supporting languages and package formats including npm, PyPI, and Maven. This makes it straightforward to integrate into existing CI/CD pipelines.
    
3. **Fine-Grained Permissions**: CodeArtifact leverages AWS Identity and Access Management (IAM) to control access to repositories. You can define precise access policies to control who can publish or modify packages.
    
4. **Upstream Sources**: You can connect your repositories to public repositories (upstreams), which enables your builds to inherit packages from public sources while storing your own artifacts securely in AWS. For instance, you can pull packages from npm public registry or Maven central and cache them in your private repository.
    
5. **Immutable Storage**: Packages stored in CodeArtifact are immutable, which means that once a version of a package is uploaded, it cannot be changed. This ensures reliability and consistency in your software builds.
    
6. **Automatic Scaling**: As a managed service, AWS CodeArtifact scales automatically to handle any number of requests and the storage of artifacts, removing the need for manual scaling of infrastructure.
    

### How It Works

- **Create a Domain**: In CodeArtifact, a domain is a container for repositories. First, create a domain which will contain all your repositories.
    
- **Create Repositories**: Within the domain, create one or more repositories. Repositories can be configured to store specific types of artifacts, such as npm packages or Maven artifacts.
    
- **Configure Upstream Sources**: Set up connections to upstream sources if you want to pull packages from external public repositories and cache them in your CodeArtifact repository.
    
- **Define Access Policies**: Use AWS IAM to define who can access your repositories and what actions they can perform, such as publishing new packages or downloading existing ones.
    
- **Publish and Consume Packages**: Developers can publish new versions of packages to these repositories and include them as dependencies in their projects using standard package management tools.
    

### Benefits

- **Centralized Management**: Provides a centralized, scalable service to manage artifacts across your development teams, improving efficiency and standardization.
    
- **Enhanced Security**: Offers robust security features, including fine-grained permissions and integration with AWS IAM, ensuring that artifacts are protected.
    
- **High Availability**: As a managed service, AWS ensures high availability and durability of the repositories, so you don’t have to worry about the underlying infrastructure.
    
- **Reduced Latency**: By caching external packages locally within AWS, you can reduce latency and improve build times in your development and deployment processes.
    

### Use Cases

- **Software Development**: Any organization developing software can use AWS CodeArtifact to manage third-party packages and their own developed packages securely and efficiently.
    
- **Build and Release Management**: Integrate CodeArtifact into CI/CD pipelines to manage dependencies reliably during automated builds and deployments.
    
- **Multi-team Development**: Large organizations with multiple development teams can use CodeArtifact to share common packages across teams while maintaining strict access and version control.
    

AWS CodeArtifact provides a robust solution for artifact management, helping organizations streamline their development and deployment workflows while maintaining high levels of security and compliance.