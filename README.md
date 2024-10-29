# AWS-CI-CD-PIPELINE
# CI/CD Pipeline for NGINX Deployment on EC2 using AWS Services

![362878718-b8162366-e7e6-4370-af7f-97e6edbec0b9](https://github.com/user-attachments/assets/4268c1ef-7f81-4690-881f-ced279189936)


Welcome to the **CI/CD Pipeline for NGINX Deployment** project! This repository contains everything you need to set up a fully automated CI/CD pipeline using AWS services such as CodeCommit, CodeBuild, CodeDeploy, and S3. This pipeline automates the process of building, testing, and deploying applications on AWS.



##  **Project Overview**

This project automates the deployment of an NGINX web server on an EC2 instance using the following AWS services:

- **CodeCommit**: Version control for storing source code and configuration files.
- **CodeBuild**: Compiles and builds the project.
- **Git Installed**: Git must be installed and configured to manage version control in the VS 
      Code environment. 
- **S3**: Stores build artifacts.
- **CodeDeploy**: Deploys the application to the EC2 instance.

## 🛠️ **Key Features**

- **Automated Deployments**: Push code changes to CodeCommit, and the pipeline automatically builds and deploys them.
- **NGINX Web Server**: Set up and configure NGINX on an EC2 instance using scripts.
- **Scalable Architecture**: Easily scalable to meet the needs of your application.

## 🔧 **Setup Instructions**

### 1. **Clone the Repository**
  - Clone Repository to Local Machine: 
  - In the CodeCommit console, open the repository you created. 
  - Click Clone URL and copy the HTTPS URL.
  - Open Visual Studio Code terminal and run: 
  ```bash
   git clone https://git-codecommit.<region>.amazonaws.com/v1/repos/MyAppRepo
   ```

### 3.**Download git**
     
     - Git –version 
     -If not downloaded make sure to download from official website

### 2. **Create and Configure AWS Services**
   - **CodeCommit**: Store your source code.
   - **CodeBuild**: Build and package your application.
   - **S3**: Store your build artifacts.
   - **CodeDeploy**: Automate your deployment process.
   - 

### 3. **Install CodeDeploy Agent on EC2**
   - Install and start the CodeDeploy agent on your EC2 instance.

### 4. **Push Code to CodeCommit**
   - Add and commit your files, then push them to the repository.

### 5. **Deploy and Monitor**
   - Monitor the deployment process and receive email notifications.

##  **Configuration Files**

### **`buildspec.yml`**
Defines the build process for CodeBuild.

### **`appspec.yml`**
Specifies the deployment steps for CodeDeploy.

### **Scripts**
- **`install_nginx.sh`**: Installs NGINX on the EC2 instance.
- **`start_nginx.sh`**: Starts the NGINX service.
