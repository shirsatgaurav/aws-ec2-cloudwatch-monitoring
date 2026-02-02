# aws-ec2-cloudwatch-monitoring
Hands-on AWS project to monitor EC2 instances using CloudWatch, create CPU alarms, and send email alerts via SNS.

# AWS EC2 CloudWatch Monitoring & Alerting

## 📌 Project Overview
This project demonstrates a hands-on implementation of monitoring and alerting for an Amazon EC2 instance using AWS CloudWatch.  
Is project ka goal EC2 instance ke CPU usage ko monitor karna aur threshold cross hone par email alert receive karna hai.

---

## 🛠️ Services & Tools Used
- Amazon EC2
- AWS CloudWatch
- CloudWatch Agent
- Amazon SNS
- IAM Role
- Amazon Linux
- Stress Tool (for testing)

---

## 🧱 Architecture
EC2 instance par CloudWatch Agent install kiya gaya hai jo metrics CloudWatch ko send karta hai.  
CloudWatch Alarm CPU utilization threshold cross hone par SNS topic trigger karta hai jo email alert bhejta hai.


---

## ⚙️ Implementation Steps
1. EC2 instance launch ki with IAM role attached  
2. CloudWatch Agent install & configure kiya  
3. CPU Utilization ke liye CloudWatch Alarm create ki  
4. SNS topic create karke email subscription add ki  
5. Stress tool use karke CPU load generate kiya  

---

## 🧪 Testing & Validation
CPU load generate karne ke liye niche diya command use kiya gaya:

```bash
stress --cpu 2 --timeout 300


