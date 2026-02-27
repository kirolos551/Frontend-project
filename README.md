
# Frontend Static Website with Automated CI/CD

## 📖 Project Overview
This is a static frontend project built using:
- HTML5
- CSS3
- JavaScript

The project demonstrates how to implement a full CI/CD pipeline using GitHub Actions to automatically deploy updates to a production Ubuntu server.

---

## 🚀 Live Deployment Architecture

Developer → Push to GitHub → GitHub Actions → SSH → Ubuntu Server → Nginx → Live Website

---

## ⚙️ Tech Stack

- HTML / CSS / JavaScript
- Git & GitHub
- GitHub Actions (CI/CD)
- Ubuntu Server
- Nginx
- SSH & Rsync
---
## 🔄 CI/CD Pipeline

The deployment process is fully automated:

- Any push to the `main` branch triggers GitHub Actions
- The workflow connects securely to the Ubuntu server via SSH
- Files are synchronized using `rsync`
- The website updates automatically without manual intervention.

Workflow file location:

.github/workflows/deploy.yml
---

## 🔐 Secrets Configuration

The following GitHub repository secrets are required:

- `SERVER_IP`
- `SERVER_USER`
- `SSH_PRIVATE_KEY`

---

## 🖥️ Server Setup

Ubuntu Server configured with:

- Nginx installed
- Web root directory:
  /var/www/frontend

Permissions configured for deployment user.
------
## 📂 Project Structure
Frontend-project /
│
├── index.html
├── style.css
├── script.js
└── .github/
└── workflows/
└── deploy.yml
------
##  Why This Project ?

This project highlights :

- Practical DevOps skills
- CI/CD Automation
- Secure SSH-based deployments
- Production-style server setup
- Real-world deployment workflow
----
## 👨‍💻 Author
CI/CD  pipeline, deployment automation, and server configuration implemented by:
kirolos  
DevOps Engineer
