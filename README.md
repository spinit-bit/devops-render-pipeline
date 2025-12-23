# 🚀 Automated GitOps Deployment Pipeline

![Python](https://img.shields.io/badge/Python-3.9-blue?style=for-the-badge&logo=python)
![Docker](https://img.shields.io/badge/Docker-Container-2496ED?style=for-the-badge&logo=docker)
![Render](https://img.shields.io/badge/Render-Cloud-black?style=for-the-badge&logo=render)
![Status](https://img.shields.io/badge/Status-Deployed-success?style=for-the-badge)

**Live Demo:** [Click Here to See the App](https://devops-pipeline-app.onrender.com/)

## 📖 Project Overview
This project demonstrates a modern **GitOps** workflow. It is a containerized Python web application that automatically builds and deploys to the cloud whenever code is pushed to the repository.

Instead of manual server configuration, this project uses **Infrastructure as Code (IaC)** and **Docker** to ensure consistency between development and production environments.

## 🏗️ Architecture


**The Workflow:**
1.  **Code:** Development is done locally in VS Code using Python (Flask).
2.  **Containerize:** A `Dockerfile` packages the app and dependencies into a lightweight image.
3.  **Version Control:** Code is pushed to **GitHub**.
4.  **CI/CD Trigger:** **Render** detects the push event immediately.
5.  **Build & Deploy:** Render pulls the code, builds the Docker container, and deploys it to a live server environment.

## 🛠️ Tech Stack
* **Language:** Python (Flask Framework)
* **Containerization:** Docker
* **Cloud Platform:** Render (PaaS)
* **Infrastructure as Code:** Render Blueprints (YAML)
* **Version Control:** Git & GitHub

## 📂 Project Structure
```bash
├── app.py              # The main Flask application
├── Dockerfile          # Instructions to build the container image
├── render.yaml         # IaC blueprint for cloud deployment
├── requirements.txt    # Python dependencies
└── README.md           # Project documentation
