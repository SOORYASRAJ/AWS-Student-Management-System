# ☁️ AWS Student Management System

<p align="center">
  <b>A cloud-based Student Management System deployed using AWS services</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/AWS-Cloud-orange?logo=amazonaws&logoColor=white">
  <img src="https://img.shields.io/badge/Python-Flask-blue?logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/MySQL-Database-blue?logo=mysql&logoColor=white">
  <img src="https://img.shields.io/badge/Linux-EC2-black?logo=linux&logoColor=white">
  <img src="https://img.shields.io/badge/Amazon-S3-red?logo=amazons3&logoColor=white">
  <img src="https://img.shields.io/badge/AWS-Lambda-orange?logo=awslambda&logoColor=white">
</p>

---

## 📌 About the Project

The **AWS Student Management System** is a web-based application developed using **Python Flask** and deployed on **Amazon Web Services (AWS)**.

The application provides a login system and allows users to access and manage student information stored in a **MySQL database hosted on Amazon RDS**.

The project demonstrates the deployment of a web application using multiple AWS services including **VPC, EC2, RDS, S3, Lambda, Application Load Balancer, and CloudWatch**.

---

## 🏗️ Architecture

The following architecture demonstrates the AWS infrastructure used to deploy the Student Management System.

![AWS Student Management System Architecture](screenshots/aws-architecture.png)


| AWS Service                   | Purpose                                                        |
| ----------------------------- | -------------------------------------------------------------- |
| **Amazon VPC**                | Creates an isolated network environment                        |
| **Amazon EC2**                | Hosts the Flask web application                                |
| **Amazon RDS**                | Hosts the MySQL database                                       |
| **Application Load Balancer** | Receives and distributes application traffic                   |
| **Amazon S3**                 | Stores uploaded files/images                                   |
| **AWS Lambda**                | Performs event-driven processing when files are uploaded to S3 |
| **Amazon CloudWatch**         | Monitors AWS resources and application infrastructure          |
| **Security Groups**           | Controls inbound and outbound network traffic                  |

✨ Features
🔐 User login authentication
👨‍🎓 Student information management
🗄️ MySQL database integration
☁️ AWS cloud deployment
📦 File storage using Amazon S3
⚡ Event-driven Lambda function
⚖️ Application Load Balancer
📊 CloudWatch monitoring
🔒 Network security using Security Groups
🌐 VPC-based AWS infrastructure

🛠️ Technologies
Application
<p> <img src="https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white"> <img src="https://img.shields.io/badge/Flask-Web%20Framework-black?logo=flask&logoColor=white"> <img src="https://img.shields.io/badge/HTML5-orange?logo=html5&logoColor=white"> <img src="https://img.shields.io/badge/CSS3-blue?logo=css3&logoColor=white"> </p>
Database
<p> <img src="https://img.shields.io/badge/MySQL-Database-blue?logo=mysql&logoColor=white"> </p>
Cloud
<p> <img src="https://img.shields.io/badge/Amazon%20EC2-orange?logo=amazonec2&logoColor=white"> <img src="https://img.shields.io/badge/Amazon%20RDS-blue?logo=amazonrds&logoColor=white"> <img src="https://img.shields.io/badge/Amazon%20S3-red?logo=amazons3&logoColor=white"> <img src="https://img.shields.io/badge/AWS%20Lambda-orange?logo=awslambda&logoColor=white"> <img src="https://img.shields.io/badge/AWS%20VPC-purple?logo=amazonaws&logoColor=white"> <img src="https://img.shields.io/badge/CloudWatch-orange?logo=amazoncloudwatch&logoColor=white"> </p>

Application Workflow

1️⃣ User opens the application
              ↓
2️⃣ Application Load Balancer receives the request
              ↓
3️⃣ ALB forwards request to EC2
              ↓
4️⃣ Flask application processes the request
              ↓
5️⃣ Application connects to RDS MySQL
              ↓
6️⃣ Login / student data is retrieved
              ↓
7️⃣ Response is displayed to the user


## 🗄️ Database

The application uses **MySQL hosted on Amazon RDS**.

### Users Table

Used to store user authentication information.


users
├── id
├── username
└── password
students
├── student details
└── academic / personal information

![Login Page](screenshots/login.png)

![Student Management Page](screenshots/student.png)
