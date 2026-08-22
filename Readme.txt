# MyResume - DevOps CI/CD Project

A personal resume website deployed using AWS, Docker, Jenkins, SonarQube and Docker Hub.

## 🚀 Project Overview

This project demonstrates a complete CI/CD pipeline for deploying a static resume website.

Whenever code is pushed to GitHub, Jenkins performs code analysis, builds a Docker image, tests the container and pushes the image to Docker Hub.

The application is then deployed on an AWS EC2 instance using Docker.

## 🛠️ Tools & Technologies

- AWS EC2
- Terraform
- Git & GitHub
- Jenkins
- SonarQube Community Build
- Docker
- Docker Hub
- Linux
- Nginx
- HTML
- CSS
- JavaScript

## 🔄 CI/CD Pipeline

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

## ☁️ AWS Infrastructure

The infrastructure was created using Terraform.

### EC2 Instances

- Jenkins Server
- SonarQube Server
- Application Server

## 🔍 SonarQube

SonarQube is integrated with Jenkins for static code analysis and quality checks.

## 🐳 Docker

The resume website is containerized using Docker and served using Nginx.

## 📦 Docker Hub

The Docker image is pushed to Docker Hub:

`shubhmohare/myresume:latest`

## 🎯 Key Features

- Infrastructure provisioning using Terraform
- CI/CD using Jenkins
- Static code analysis using SonarQube
- Docker containerization
- Docker image publishing
- Application deployment on AWS EC2
- Automated testing of the Docker container

## 📸 Project Screenshots

### Jenkins Pipeline

![Jenkins Pipeline](screenshots/jenkins-pipeline.png)

### SonarQube Analysis

![SonarQube](screenshots/sonarqube.png)

### Docker Hub

![Docker Hub](screenshots/dockerhub.png)

### Deployed Website

![Website](screenshots/website.png)

## 👨‍💻 Author

Shubham Mohare
