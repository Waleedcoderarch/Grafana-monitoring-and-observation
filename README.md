# Grafana Monitoring and Observation

## 📌 Project Overview
This project demonstrates a comprehensive cloud monitoring solution built using **AWS CloudWatch** and **Grafana**. The dashboard provides real-time visibility into system performance, traffic patterns, scaling behavior, and application health across multiple AWS services.

The main goal of this project is to create a **centralized monitoring dashboard** that helps track infrastructure metrics and detect performance issues efficiently.

---

## 🚀 Features

- Real-time monitoring of EC2 CPU utilization and network traffic  
- Auto Scaling Group capacity tracking (Desired vs In-Service instances)  
- Application Load Balancer request monitoring  
- Target group health status visualization (Healthy and Unhealthy targets)  
- EBS disk performance monitoring  
- AWS Lambda function invocation and error tracking  
- CloudWatch alarm visualization for CPU utilization  
- Interactive dashboard with dynamic instance selection using Grafana variables  

---

## 🛠️ Technologies Used

- **Amazon Web Services (AWS)**
  - EC2
  - Auto Scaling Group (ASG)
  - Application Load Balancer (ALB)
  - Elastic Block Store (EBS)
  - Lambda
  - CloudWatch

- **Grafana**
  - Dashboard creation
  - CloudWatch data source integration
  - Visualization panels
  - Dashboard variables

---

## 📊 Metrics Monitored

- EC2 CPU Utilization  
- EC2 Network In and Network Out  
- EBS Read and Write Operations  
- ALB Request Count  
- Target Group Healthy and Unhealthy Host Count  
- ASG GroupDesiredCapacity and GroupInServiceInstances  
- Lambda Invocations and Errors  
- CloudWatch Alarm State  

---

## ⚙️ Architecture Overview

The monitoring setup follows this flow:

User Traffic → Application Load Balancer → Target Group → EC2 Instances  
CloudWatch collects metrics → Grafana fetches and visualizes metrics  

---

## 🧪 Testing and Validation

- Stress testing was performed on EC2 instances to simulate high CPU load  
- Auto Scaling behavior was observed under increased traffic  
- CloudWatch alarms were triggered and visualized in Grafana  
- Network and disk activity were monitored during workload simulation  

---

## 📷 Dashboard Preview

<img width="1536" height="2511" alt="Waleed-Grafana ( dashboard )-1769715704289" src="https://github.com/user-attachments/assets/957cebba-fab7-4b38-8604-700d97c98409" />


---

## 🎯 Learning Outcomes

Through this project, I learned:

- How to integrate AWS CloudWatch with Grafana  
- How to create dynamic dashboards using variables  
- How to monitor cloud infrastructure performance  
- How Auto Scaling and Load Balancing work in real-time  
- How to create and visualize CloudWatch alarms  

---

## 📌 Future Improvements

- Add alert notifications using SNS and Slack integration  
- Add custom application-level metrics  
- Improve dashboard UI with more visual indicators  

- Implement log monitoring using CloudWatch Logs  

---

## 👤 Author

**Waleed Ahmed**  
Cloud & DevOps Enthusiast  

---


