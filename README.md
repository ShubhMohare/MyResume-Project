# 🚀 MyResume — AWS DevOps CI/CD Project

> A personal resume website deployed using AWS, Docker, Jenkins, SonarQube and Terraform.

## 📌 Project Overview

MyResume is a personal resume website that I containerized using Docker and deployed on AWS EC2.

This project demonstrates a practical DevOps workflow using GitHub, Jenkins, SonarQube, Docker, Docker Hub, Terraform and Linux.

## 🏗️ Architecture

```text
GitHub
   ↓
Jenkins
   ↓
SonarQube Analysis
   ↓
Docker Build
   ↓
Docker Test
   ↓
Docker Hub
   ↓
AWS EC2
   ↓
MyResume Website
🛠️ Technologies Used
☁️ AWS EC2
🏗️ Terraform
🔧 Jenkins
🔍 SonarQube
🐳 Docker
📦 Docker Hub
🐙 GitHub
🌿 Git
🐧 Linux
🌐 Nginx
💻 HTML / CSS / JavaScript
☁️ AWS Infrastructure

The project uses separate EC2 servers for:

Jenkins Server — CI/CD automation
SonarQube Server — Code quality analysis
Application Server — Runs the Dockerized application

Infrastructure was managed using Terraform.

🔄 Jenkins CI/CD Pipeline

The Jenkins pipeline performs:

Checkout source code from GitHub
SonarQube code analysis
Docker image build
Docker container testing
Docker image push to Docker Hub
🔍 SonarQube

SonarQube is integrated with Jenkins for automated code-quality analysis.

The project successfully passed the SonarQube Quality Gate.

🐳 Docker

The application is containerized using Docker and served using Nginx.

Build
docker build -t myresume:latest .
Run
docker run -d --name myresume -p 80:80 myresume:latest
📦 Docker Hub

Docker image:

shubhmohare/myresume:latest

📸 Project Screenshots
🔧 Jenkins CI/CD Pipeline

🔍 SonarQube Quality Gate

🌐 Deployed MyResume Website

🎯 Key DevOps Concepts
Infrastructure as Code with Terraform
CI/CD with Jenkins
Static code analysis with SonarQube
Docker containerization
Docker image management
Git and GitHub workflow
Linux server administration
AWS EC2 deployment
Jenkins Pipeline as Code
Automated Docker testing
💡 What I Learned

This project gave me hands-on experience with:

AWS
Terraform
Jenkins
SonarQube
Docker
Docker Hub
Git & GitHub
Linux
CI/CD
Cloud deployment
👨‍💻 Author
Shubham Mohare

Aspiring AWS & DevOps Engineer

AWS • DevOps • Terraform • Docker • Kubernetes • Jenkins • Linux

⭐ Thanks for checking out my project!