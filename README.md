# CarePlus – End-to-End AWS Data Engineering Project

![AWS Data Pipeline](project-care-plus/pipeline%20architecture.png)



---

## 📘 Project Overview

**CarePlus** is a complete **AWS-based data engineering and analytics project** that processes support ticket and system log data using an automated **ETL pipeline**.  
The project demonstrates the integration of multiple AWS services for **data ingestion, transformation, storage, querying, and visualization**, enabling business teams to monitor **system health and customer support performance** in real-time.

---

## 🎯 Objective

To build a **scalable cloud-based data pipeline** for CarePlus that:
- Collects raw ticket and log data from multiple sources.
- Cleanses, transforms, and stores it in AWS.
- Supports analytical insights through **Athena queries** and **Power BI dashboards**.
- Enables monitoring of **system performance**, **agent efficiency**, and **support issue trends**.

---

## ☁️ AWS Architecture

| Layer | AWS Service | Description |
|-------|--------------|--------------|
| **Storage** | 🪣 **Amazon S3** | Stores raw and transformed data. Acts as a data lake. |
| **Compute / ETL** | 🧩 **AWS Lambda** | Performs data ingestion and transformation tasks automatically. |
| **Data Processing** | 🔥 **AWS Glue** | Handles schema inference, ETL transformations, and data cataloging. |
| **Query Engine** | 🔍 **Amazon Athena** | Enables SQL-based analysis on transformed data stored in S3. |
| **Data Warehouse** | 🏗️ **Amazon Redshift** | Stores structured analytical data for advanced querying. |
| **Visualization** | 📊 **Power BI** | Connects with Redshift to visualize performance metrics. |

---

## 🔄 End-to-End Workflow

1. **Raw Data Ingestion**  
   - Ticket data and support logs uploaded to **Amazon S3 (Raw Zone)**.  
2. **Triggering Lambda**  
   - New uploads trigger **AWS Lambda** for initial validation and cleanup.  
3. **Data Transformation (ETL)**  
   - **AWS Glue** jobs perform advanced transformations and schema mapping.  
4. **Data Querying**  
   - Transformed data stored in **S3 (Processed Zone)** is queried via **Athena**.  
5. **Data Warehousing**  
   - Final datasets are loaded into **Amazon Redshift** for high-performance analytics.  
6. **Dashboard Visualization**  
   - **Power BI Dashboard** displays **agent performance, issue trends, and system metrics**.

---

## 📊 Power BI Dashboard Highlights

**Dashboard Title:** *CarePlus Ticket & System Insights*

| Metric | Description |
|---------|--------------|
| 🧑‍💼 **Total Agents:** | 5 active support agents |
| 🧾 **Total Tickets:** | 587 tickets processed |
| ✅ **Resolved Tickets:** | 474 (80.7%) |
| 🕑 **Average Resolution Time:** | 1077 minutes |
| ⚙️ **Average CPU Utilization:** | 49.67% |
| ⏱️ **Average Response Time:** | 977.53 ms |

### 🔍 Key Insights
- **Top Performing Agent:** *Rohit* handled the highest number of tickets (128).  
- **Most Frequent Issues:** *Feature Request* and *Payment Failure* categories dominate ticket volume.  
- **Priority Mix:** Majority of issues fall under *Medium* and *Low* priority.  
- **Escalation Rate:** Only ~3.7% of tickets required escalation.  
- **System Health:** CPU usage peaked near 90% on July 20, 2025, during high request loads.  

---

## 🧠 Learning Outcomes

- Designed and deployed a **serverless ETL pipeline** on AWS.  
- Implemented **data lake architecture** using S3, Glue, and Athena.  
- Built an **automated reporting system** with Power BI connected to Redshift.  
- Applied **data transformation and aggregation techniques** for real-time analytics.  
- Learned best practices for **AWS cost optimization and automation**.

---

## 🧰 Tools & Technologies

| Category | Tools Used |
|-----------|-------------|
| **Cloud Platform** | AWS |
| **Services** | S3, Lambda, Glue, Athena, Redshift |
| **Visualization** | Power BI |
| **Languages** | Python, SQL |
| **Architecture** | Serverless Data Pipeline |
| **Version Control** | Git & GitHub |

---


