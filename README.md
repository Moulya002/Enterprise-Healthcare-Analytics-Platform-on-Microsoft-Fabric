# 🏥 Enterprise Healthcare Analytics Platform using Microsoft Fabric

An end-to-end Data Engineering project built on **Microsoft Fabric** using the **Medallion Architecture (Bronze → Silver → Gold)**.

In this project, I built a healthcare analytics pipeline that ingests raw healthcare datasets, cleans and transforms the data using PySpark, automates the workflow with Microsoft Fabric Pipelines, and prepares business-ready datasets for reporting in Power BI.

---

## 🚀 Project Overview

The project follows the Medallion Architecture:

```text
Raw CSV Files
      │
      ▼
Bronze Layer
      │
      ▼
Silver Layer
      │
      ▼
Gold Layer
      │
      ▼
Power BI Dashboard
```

### Bronze Layer
Stores the raw healthcare data exactly as received.

### Silver Layer
Cleans, standardizes, and validates the data.

### Gold Layer
Creates business-ready tables for analytics and reporting.

---

## 🛠 Tech Stack

- Microsoft Fabric
- OneLake
- Lakehouse
- PySpark
- Spark SQL
- Delta Lake
- Microsoft Fabric Pipelines
- Power BI
- Python
- SQL
- Git & GitHub

---

## 📂 Project Structure

```text
Enterprise-Healthcare-Analytics-Platform/

├── 01_Bronze_Ingestion.ipynb
├── 02_Silver_Transformation.ipynb
├── 03_Gold_Transformation.ipynb
├── README.md
└── LICENSE
```

---

## 📊 Dataset

This project uses publicly available healthcare datasets containing:

- Hospital Information
- Provider Services
- Unplanned Hospital Visits

The data is loaded into Microsoft Fabric Lakehouse and processed through the Bronze, Silver, and Gold layers.

---

## 🥉 Bronze Layer

The Bronze layer stores the raw data without making any changes.

### What I did

- Loaded CSV files into Microsoft Fabric Lakehouse
- Created Bronze Delta tables
- Preserved the original data for future processing

### Tables

- bronze_hospital_information
- bronze_provider_services
- bronze_unplanned_hospital_visits

---

## 🥈 Silver Layer

The Silver layer focuses on preparing clean and reliable data.

### Transformations

- Removed duplicate records
- Handled missing values
- Standardized column names
- Converted data types
- Applied basic data quality checks

### Output Table

- hospital_silver

---

## 🥇 Gold Layer

The Gold layer contains curated datasets that are ready for reporting.

### Gold Tables

- gold_birth_friendly
- gold_emergency_services
- gold_hospital_ownership
- gold_hospital_type
- gold_state_summary
- gold_top_hospitals

These tables are optimized for analytics and Power BI dashboards.

---

## 🔄 Data Pipeline

The entire workflow is orchestrated using Microsoft Fabric Pipelines.

```text
Bronze Ingestion
        │
        ▼
Silver Transformation
        │
        ▼
Gold Transformation
```

Each notebook runs in sequence to ensure the data flows smoothly through each layer.

---

## 📈 Power BI Dashboard

The dashboard is built using the Gold layer tables and includes insights such as:

- Hospital distribution by state
- Top-rated hospitals
- Emergency service availability
- Birth-friendly hospitals
- Hospital ownership analysis

> *(Dashboard screenshots will be added soon.)*

---

## 💡 Skills Demonstrated

- Microsoft Fabric
- OneLake & Lakehouse
- PySpark
- Spark SQL
- Delta Lake
- ETL Pipeline Development
- Medallion Architecture
- Data Cleaning & Transformation
- Microsoft Fabric Pipelines
- Power BI
- Git & GitHub

---

## 📚 What I Learned

Working on this project helped me gain hands-on experience with Microsoft Fabric and modern data engineering practices. I learned how to build an end-to-end data pipeline, organize data using the Medallion Architecture, automate workflows with Fabric Pipelines, and prepare clean datasets for business reporting.

---

## 👨‍💻 Author

**Moulya Reddygari Bhupal**

- GitHub: https://github.com/Moulya002
- LinkedIn: https://www.linkedin.com/in/moulyarb/

---

⭐ If you found this project useful, feel free to give it a star!
