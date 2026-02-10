# 🚀 CI/CD Pipeline for 2048 Game using AWS

This repository demonstrates how to deploy the **2048 Game** using a **fully automated CI/CD pipeline** on AWS. The pipeline handles building, testing, and deploying a Dockerized application using modern AWS DevOps services.

---

## 📌 Project Overview

This project implements an end-to-end **CI/CD pipeline** to automate the deployment of a containerized 2048 game on AWS. The pipeline ensures faster releases, consistent builds, and reliable deployments by leveraging managed AWS services.

**Key goals:**
- Automate build and deployment workflows
- Use serverless container orchestration with ECS Fargate
- Follow DevOps best practices for containerized applications

![git_readme](https://github.com/user-attachments/assets/5f913bde-83a4-4cb3-8e0a-3561110050dc)

---

## 🔧 Key Features

- **Dockerized Application** – The 2048 game is containerized using Docker.
- **Automated CI/CD Pipeline** – Code changes trigger automatic build and deployment.
- **Serverless Containers** – Deployed on Amazon ECS using the Fargate launch type.
- **Secure & Scalable** – IAM roles and managed AWS services ensure security and scalability.

---

## 🧩 Architecture Overview

1. Code is pushed to **GitHub**
2. **AWS CodePipeline** triggers the pipeline
3. **AWS CodeBuild** builds the Docker image
4. Docker image is pushed to **Amazon ECR**
5. **Amazon ECS (Fargate)** deploys the updated container

---

## 👩‍💻 Steps Performed

### 1️⃣ Set Up ECS Cluster & ECR Repository
- Create an Amazon ECS cluster using the Fargate launch type
- Create an Amazon ECR repository to store Docker images

### 2️⃣ Prepare the 2048 Game Code
- Clone and structure the game source code
- Create a Dockerfile for containerization

### 3️⃣ Configure AWS CodeBuild (Continuous Integration)
- Automatically build Docker images on every code change
- Push built images to Amazon ECR

### 4️⃣ Configure AWS CodePipeline (Continuous Deployment)
- Create an end-to-end CI/CD pipeline
- Automate deployment to Amazon ECS after successful builds

---

## 🛠 AWS Services Used

- **AWS CodePipeline** – Orchestrates the CI/CD workflow  
- **AWS CodeBuild** – Builds and tests Docker images  
- **Amazon ECR** – Stores and manages Docker images  
- **Amazon ECS (Fargate)** – Runs containers without managing servers  
- **IAM Roles & Policies** – Provides secure service-to-service access  

---

## 🧰 Tools Used

`AWS CodePipeline` · `AWS CodeBuild` · `Amazon ECS` · `Amazon ECR` · `Docker` · `GitHub`

---

## 🚀 Getting Started

1. Fork this repository  
2. Clone the repository locally  
3. Configure AWS credentials  
4. Create required AWS resources (ECR, ECS, CodeBuild, CodePipeline)  
5. Push code changes to trigger the CI/CD pipeline  
