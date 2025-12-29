🚀 Kubernetes Backend Deployment on Amazon EKS
📌 Project Overview

This project demonstrates how to containerize a backend application, store the image securely in Amazon ECR, and deploy it to a Kubernetes cluster running on Amazon EKS. It showcases real-world DevOps workflows including containerization, Kubernetes orchestration, AWS integration, and troubleshooting deployment issues.

The goal of this project is to understand how applications move from code → container → cluster, and how Kubernetes manages deployments at scale.

🛠️ Tools & Technologies

AWS: EKS, EC2, ECR, IAM

Containers: Docker

Orchestration: Kubernetes

CLI Tools: kubectl, eksctl, AWS CLI

OS: Linux (Kali / Amazon Linux)

🏗️ Architecture

Backend application packaged into a Docker image

Image pushed to Amazon ECR

Kubernetes Deployment manages application pods

Kubernetes Service (NodePort) exposes the app externally

EKS worker nodes run container workloads

⚙️ Key Steps Implemented
1️⃣ Containerization

Built a Docker image for the backend application using a Dockerfile

Tagged and pushed the image to Amazon ECR

2️⃣ Kubernetes Cluster Setup

Created an EKS cluster using eksctl

Configured IAM roles and access

Verified cluster and node health using kubectl

3️⃣ Kubernetes Manifests

Created a Deployment manifest to manage backend pods

Created a Service manifest (NodePort) to expose the application

4️⃣ Deployment & Verification

Applied manifests using kubectl

Verified pod scheduling and node readiness

Troubleshot pending pods caused by node capacity constraints

Successfully accessed the application via NodePort

🧠 Challenges & Lessons Learned

Learned how Kubernetes scheduling works and why pods can remain in a Pending state

Understood node capacity limits and how resource requests affect scheduling

Gained hands-on experience troubleshooting real Kubernetes deployment issues

Improved understanding of how EKS integrates with AWS IAM and ECR



🎯 Key Takeaways

Kubernetes abstracts infrastructure complexity but requires proper configuration

Container registries are essential for scalable deployments

Troubleshooting is a core DevOps skill, not an edge case

This project reflects real-world cloud-native deployment practices

👤 Author

Victor Eze
Cloud & DevOps Engineer
