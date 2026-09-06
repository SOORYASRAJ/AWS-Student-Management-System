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

```text
                         🌐 User
                           │
                           ▼
                 ┌───────────────────┐
                 │ Application       │
                 │ Load Balancer     │
                 │      (ALB)        │
                 └─────────┬─────────┘
                           │
                           ▼
                 ┌───────────────────┐
                 │      EC2          │
                 │  Flask Web App    │
                 └─────────┬─────────┘
                           │
                           ▼
                 ┌───────────────────┐
                 │      RDS          │
                 │   MySQL Database  │
                 └───────────────────┘

                     ┌─────────────┐
                     │     S3      │
                     │ File Storage│
                     └──────┬──────┘
                            │
                            ▼
                     ┌─────────────┐
                     │   Lambda    │
                     │ Event-based │
                     │ Processing  │
                     └─────────────┘

                     ☁️ CloudWatch
                     Monitoring
