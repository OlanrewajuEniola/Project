# Jenkins-Maven-Tomcat CI/CD Pipeline Project

This project demonstrates a complete Continuous Integration and Continuous Deployment (CI/CD) pipeline using **Jenkins**, **Maven**, and **Apache Tomcat** on an **Ubuntu EC2 instance**. It showcases my foundational DevOps skills and is part of my journey toward becoming a DevOps Engineer.

## 🔧 Tech Stack

- **Jenkins** – Automation server for CI/CD
- **Maven** – Build tool for compiling Java WAR applications
- **Apache Tomcat** – Application server for deploying WAR files
- **Git & GitHub** – Source control and webhook trigger
- **Ubuntu EC2 (AWS)** – Hosting the Tomcat server
- **Java** – Web application language (packaged as WAR)
- **Shell Scripting** – Used for job configuration and deployment

---

## 📁 Project Structure

coco/
├── pom.xml
├── devops.txt
└── src/
└── main/
└── webapp/
└── WEB-INF/
└── web.xml


- `pom.xml` – Maven configuration for building the WAR file.
- `web.xml` – Minimal deployment descriptor for the web application.
- `devops.txt` – Notes and logs of the DevOps process.

---

## 🚀 CI/CD Pipeline Overview

### 1. Source Code Management
- Code is version-controlled in GitHub.
- Jenkins pulls the latest code via webhook or polling.

### 2. Build Process (Maven)
- Jenkins runs `mvn clean package` to compile and package the Java web app into a WAR file.

### 3. Deployment to Apache Tomcat
- Jenkins uses shell commands to:
  - SCP the WAR file to the Tomcat `webapps/` directory on the remote EC2 Ubuntu server.
  - Restart Tomcat to deploy the updated application.

---

## ✅ Completed Features

- [x] Jenkins server installed and configured on local machine
- [x] Jenkins job created to:
  - Pull code from GitHub
  - Use Maven to build WAR
  - Deploy to Tomcat on remote EC2
- [x] Webhook integration between GitHub and Jenkins
- [x] WAR deployment verified via browser and Tomcat Manager
- [x] Source code hosted publicly on GitHub

---

## 📸 Screenshot (Optional)

*(You can add a screenshot showing your Jenkins pipeline or Tomcat deployment page if you have one.)*

---

## 🧠 Key Learnings

- Configuring CI/CD pipelines with Jenkins from scratch
- Automating Maven builds and Tomcat deployment
- Connecting Jenkins to GitHub with webhooks
- Working with Linux servers and shell scripts
- Understanding WAR packaging and deployment

---

## 🛠️ Future Enhancements

- Add **Ansible** playbooks for provisioning Jenkins and Tomcat servers
- Use **Terraform** to automate AWS EC2 infrastructure setup
- Containerize the application using **Docker**
- Add monitoring using **Prometheus + Grafana**

---

## 🙋‍♂️ About Me

I'm Ola, an aspiring DevOps Engineer with a background in IT Support. I'm currently upskilling through hands-on DevOps projects.
📫 [LinkedIn](https://www.linkedin.com/in/ola-eniola-b60ba3236)

---

## 📜 License

This project is for educational purposes and open-source contributions. Feel free to fork or suggest improvements!

