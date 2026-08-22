# 🚀 MyResume — AWS DevOps CI/CD Project

<p align="center">
  <b>AWS • DevOps • CI/CD • Docker • Jenkins • Terraform • SonarQube</b>
</p>

<p align="center">
  A personal resume website deployed using a complete DevOps workflow on AWS.
</p>

---

## 📌 Project Overview

**MyResume** is a personal resume website that I containerized with Docker and deployed on AWS EC2.

This project demonstrates a practical DevOps workflow using **GitHub, Jenkins, SonarQube, Docker, Docker Hub, Terraform, Linux and AWS EC2**.

The goal of this project was to build a repeatable CI/CD process where source-code changes can be tested, analyzed, containerized and prepared for deployment.

---

## 🏗️ Architecture

```text
                    ┌──────────────┐
                    │    GitHub    │
                    │ Source Code  │
                    └──────┬───────┘
                           │
                           ▼
                    ┌──────────────┐
                    │    Jenkins   │
                    │    CI/CD     │
                    └──────┬───────┘
                           │
              ┌────────────┴────────────┐
              ▼                         ▼
       ┌──────────────┐          ┌──────────────┐
       │  SonarQube   │          │    Docker    │
       │ Code Quality │          │     Build    │
       └──────────────┘          └──────┬───────┘
                                       │
                                       ▼
                                ┌──────────────┐
                                │  Docker Hub  │
                                │    Registry  │
                                └──────┬───────┘
                                       │
                                       ▼
                                ┌──────────────┐
                                │   AWS EC2    │
                                │ Application  │
                                │    Server    │
                                └──────┬───────┘
                                       │
                                       ▼
                                🌐 MyResume App




 If you found this project useful, feel free to explore the repository.





 ![Jenkins Pipeline](screenshot/jenkins-pipeline.png)

![SonarQube Quality Gate](screenshot/sonarqube.png)

![MyResume Website](screenshot/website-2.png)