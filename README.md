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
- Amazon S3 bucket storage monitoring  
- Interactive dashboard with dynamic instance selection using Grafana variables  

---

## 🛠️ Technologies Used

### Amazon Web Services (AWS)

- EC2  
- Auto Scaling Group (ASG)  
- Application Load Balancer (ALB)  
- Elastic Block Store (EBS)  
- Lambda  
- Simple Storage Service (S3)  
- CloudWatch  

### Grafana

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
- S3 Bucket Size (BucketSizeBytes)  
- S3 Number of Objects (NumberOfObjects)  

---

## ⚙️ Architecture Overview

The monitoring setup follows this workflow:

User Traffic → Application Load Balancer → Target Group → EC2 Instances  
CloudWatch collects metrics → Grafana fetches and visualizes metrics  

This architecture enables centralized monitoring and real-time visibility into AWS infrastructure performance.

---

## 🧪 Testing and Validation

The following testing activities were performed:

- Stress testing on EC2 instances to simulate high CPU usage  
- Auto Scaling behavior observation during increased workload  
- CloudWatch alarm triggering and visualization in Grafana  
- Network and disk activity monitoring under load  
- Validation of S3 storage metrics  

---

## 📷 Dashboard Preview

<img width="1536" height="2511" alt="Grafana Dashboard" src="https://github.com/user-attachments/assets/957cebba-fab7-4b38-8604-700d97c98409" />

---

## 🗄️ Amazon S3 Storage Monitoring

This project also includes monitoring for **Amazon S3 bucket storage usage** using CloudWatch metrics visualized in Grafana. The dashboard tracks both **total storage size** and **number of stored objects (files)**.

### 📊 S3 Monitoring Panel Preview

<img width="1008" height="756" alt="S3 Dashboard-1769798294437" src="https://github.com/user-attachments/assets/ffc2206c-23c0-4a77-9416-b679486f9eff" />


---

### 📈 S3 Storage Metrics Explanation

The S3 monitoring panel displays the following metrics:

- **NumberOfObjects**  
  Shows the total number of files stored in the S3 bucket.  
  In this project, the bucket contains **3 objects (files)**.

- **BucketSizeBytes**  
  Represents the total storage space used by the bucket in bytes.  
  The recorded value is: 11,379,239 bytes

### 🔄 Storage Conversion Formula

To convert bytes into megabytes (MB):
1MB = 1,048,576 bytes
---

### 🧮 Calculation
11,379,239 ÷ 1,048,576 ≈ 10.86 MB
---

### ✅ Final Result

The S3 bucket is using approximately:

> **10.86 MB of storage space**

This confirms that the uploaded data is accurately reflected in both CloudWatch and Grafana.

---

### 📝 Important Note

Amazon S3 storage metrics are updated **once per day** by AWS. These metrics are not real-time and may take up to **24 hours** to reflect new uploads or deletions. This is expected behavior and part of AWS metric processing.

---

## 🎯 Learning Outcomes

Through this project, I learned:

- How to integrate AWS CloudWatch with Grafana  
- How to build centralized monitoring dashboards  
- How to monitor cloud infrastructure performance  
- How Auto Scaling and Load Balancing work in real-time  
- How to visualize CloudWatch alarms  
- How S3 storage metrics are collected and processed  

---

## 📌 Future Improvements

- Add alert notifications using SNS and Slack integration  
- Add custom application-level metrics  
- Improve dashboard UI with advanced visual indicators  
- Implement centralized log monitoring using CloudWatch Logs  

---

## 👤 Author

**Waleed Ahmed**  
Cloud & DevOps Enthusiast  

---



