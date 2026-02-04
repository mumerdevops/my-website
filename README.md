Ek zabardast README file aapki repository ka chehra hoti hai. Isse dekh kar lagta hai ke kisi professional ne kaam kiya hai.

Aap niche diye gaye text ko copy karke apni repository mein `README.md` ke naam se file banayein aur usme paste kar dein:

---

# 🚀 Automated Web Deployment on AWS EC2

Hi! I am a 15-year-old developer learning **DevOps**. This project demonstrates a fully automated **CI/CD Pipeline** using GitHub Actions to deploy a website on an AWS EC2 instance.

## 🛠 Project Overview

In this project, I have set up an automated workflow where every time I push changes to my `index.html` file, it automatically updates on my live web server.

### 🏗 Architecture

* **Local Machine:** Coding the website.
* **GitHub:** Version control and hosting the code.
* **GitHub Actions:** The "Engine" that automates the deployment.
* **AWS EC2:** The cloud server where the website is hosted.
* **Nginx:** The web server software that serves the HTML file.

---

## ⚡ Features

* **Automation:** No manual file uploading (No FileZilla/WinSCP needed).
* **Fast Deployment:** Changes reflect on the live IP within seconds.
* **Cloud Hosted:** High availability using Amazon Web Services.

---

## 🚀 How to Set This Up

### 1. EC2 Setup

* Launched an Ubuntu EC2 instance.
* Installed Nginx using: `sudo apt update && sudo apt install nginx -y`.
* Opened **Port 80** (HTTP) and **Port 22** (SSH) in Security Groups.

### 2. GitHub Secrets

To make the automation work, I added the following secrets in GitHub:

* `HOST_IP`: My EC2 Public IP.
* `EC2_SSH_KEY`: My private `.pem` key content.

### 3. CI/CD Workflow

The automation is handled by `.github/workflows/deploy.yml`. It uses **SCP** to securely transfer the files from GitHub's runner to the EC2 server path `/var/www/html/`.

---

## 📈 Next Steps (Phase 4)

* [ ] **Dockerization:** Wrap the website in a Docker container.
* [ ] **Docker Hub:** Automate image building and pushing to Docker Hub.
* [ ] **Container Orchestration:** Run the website as a container on EC2.

---

## 👨‍💻 About Me

I'm a passionate 15-year-old student exploring the world of Cloud Computing and DevOps. Follow my journey!

---

### Aapke liye agla qadam:

Aap is README file ko apni repo mein daal dein. Iske baad, agar aapka "Phase 3" (Green Tick) successfully chal raha hai, to kya hum **Phase 4 (Docker)** shuru karein?

Docker seekhna thora mushkil hai lekin ye aaj kal ki sab se bari technology hai! Batao, tayyar ho?
