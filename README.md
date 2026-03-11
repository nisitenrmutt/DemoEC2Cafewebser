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

### 📂 Step 2: Clone the Repository and Deploy
Now that the server is ready, let's pull your code from GitHub to make it live.

'**1. Navigate to the web root directory:**' (By default, Apache serves files from /var/www/html)

# Bash
cd /var/www/html
'**2. Clean up existing files:**' ⚠️ Warning: This command will permanently delete all files in the current folder.

# Bash
sudo rm -rf *
'** 3. Clone your repository:**' Run the command below to pull your project files.

(Don't forget to replace the URL with your actual Repository link!)
# Bash
sudo git clone [https://github.com/YOUR_USERNAME/YOUR_REPO.git](https://github.com/YOUR_USERNAME/YOUR_REPO.git) .
