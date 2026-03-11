# DemoEC2Cafewebser
# 🚀 Step-by-Step Guide: Web Server Installation & Git Deployment
Welcome! This guide will walk you through setting up your server and deploying your project directly from GitHub. 🛠️

---

### 📍 Step 1: Install Web Server and Git 
First, let's prepare the environment by installing Apache and Git on your server.

```bash
# Update the system to the latest version
sudo yum update -y

# Install Apache (httpd) and Git
sudo yum install httpd -y
sudo yum install git -y

# Start the Web Server and enable it to run on boot
sudo systemctl start httpd
sudo systemctl enable httpd
