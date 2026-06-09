# CI/CD Pipeline using Git, Jenkins, Docker and Kubernetes

## Overview

This project demonstrates the implementation of a Continuous Integration and Continuous Deployment (CI/CD) pipeline using GitHub, Jenkins, Docker, Docker Hub, and Kubernetes.

The pipeline automates the process of building, packaging, and deploying the application with minimal manual intervention.

---

## Technologies Used

* Python
* Flask
* GitHub
* Jenkins
* Docker
* Docker Hub
* Kubernetes
* Groovy

---

## Project Workflow

GitHub Repository
↓
Jenkins Pipeline
↓
Docker Image Build
↓
Docker Hub
↓
Kubernetes Deployment
↓
Running Application Pods

---

## Project Structure

```text
CI-CD-Assignment/
│
├── app.py
├── requirements.txt
├── Dockerfile
├── Jenkinsfile
├── deployment.yaml
├── service.yaml
├── README.md
└── .gitignore
```

---

## File Description

### app.py

Contains the Flask application code.

### requirements.txt

Stores Python dependencies required by the application.

### Dockerfile

Defines the instructions to build the Docker image.

### Jenkinsfile

Contains the Groovy pipeline script for Jenkins automation.

### deployment.yaml

Defines the Kubernetes deployment configuration.

### service.yaml

Defines the Kubernetes service configuration.

### .gitignore

Excludes unnecessary files from version control.

---

## Steps Performed

1. Created a Flask web application.
2. Containerized the application using Docker.
3. Pushed source code to GitHub.
4. Configured Jenkins pipeline using Groovy.
5. Built Docker image automatically.
6. Pushed Docker image to Docker Hub.
7. Deployed the application to Kubernetes.
8. Verified successful deployment using Kubernetes pods and services.

---

## Features

* Automated CI/CD pipeline
* Docker containerization
* Kubernetes deployment
* Scalable architecture with multiple replicas
* Error handling using Jenkins post actions
* Reusable and maintainable pipeline

---

## Output

The application was successfully deployed to Kubernetes with two running pods and exposed using a Kubernetes service.

---

## Conclusion

This project successfully demonstrates an end-to-end CI/CD pipeline using GitHub, Jenkins, Docker, Docker Hub, and Kubernetes. The automation process reduces manual effort, improves consistency, and supports scalable application deployment.
