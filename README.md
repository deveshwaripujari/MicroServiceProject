# Project Overview

## Introduction
This project demonstrates the development, deployment, and management of a microservice architecture, containerized with Docker and orchestrated using AWS Elastic Kubernetes Service (EKS). The setup includes a robust Continuous Integration/Continuous Deployment (CI/CD) pipeline facilitated by Jenkins and comprehensive unit testing via Selenium WebDriver.

## Objectives
- **Automation of Deployment**: Utilize Jenkins to automate the build and deployment processes, ensuring that updates are smoothly rolled out with minimal manual intervention.
- **Efficient Scaling**: Leverage AWS EKS to dynamically scale the application based on demand, supporting high availability and load balancing.
- **Streamlined Development Cycles**: Integrate Selenium WebDriver for continuous unit testing, reducing bugs and improving code quality throughout development phases.

## Key Components
- **Docker**: Containerization of the microservice to ensure consistent environments across development, testing, and production.
- **AWS Elastic Kubernetes Service (EKS)**: Deployment and management of containerized applications at scale, providing a highly available and resilient infrastructure.
- **Jenkins**: Automation of the CI/CD pipeline, enhancing the speed and reliability of development workflows.
- **Selenium WebDriver**: Implementation of automated tests to verify the functionality and performance of the microservice, ensuring that each release meets quality standards.

## Deployment Process
1. **Development**: Microservices are developed locally using Docker to containerize each component.
2. **Continuous Integration**: Changes are committed to the repository, triggering Jenkins to run build and test pipelines.
3. **Continuous Deployment**: Successful builds are automatically deployed to AWS EKS, where services are managed and scaled.
4. **Monitoring and Maintenance**: Ongoing monitoring and maintenance are conducted to ensure operational efficiency and to address potential issues promptly.

This project serves as a comprehensive example of modern software development practices, showcasing how cloud-native technologies can be integrated to create a resilient, scalable, and easily manageable application landscape.
