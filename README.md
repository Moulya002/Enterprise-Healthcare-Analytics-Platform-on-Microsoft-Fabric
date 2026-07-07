# 🏥 Enterprise Healthcare Analytics Platform on Microsoft Fabric

An end-to-end Data Engineering project built using **Microsoft Fabric** to process, transform, and analyze healthcare data using the **Medallion Architecture (Bronze → Silver → Gold)**. This project demonstrates modern data engineering practices including data ingestion, transformation, orchestration, Delta Lake storage, and Power BI reporting.

---

# 📌 Project Overview

This project ingests raw healthcare datasets into Microsoft Fabric Lakehouse, transforms them into clean analytical datasets, orchestrates the entire workflow using Fabric Pipelines, and prepares curated Gold tables for business intelligence and reporting.

The project follows the Medallion Architecture:

```
Raw CSV Files
      │
      ▼
Bronze Layer (Raw Data)
      │
      ▼
Silver Layer (Cleaned & Standardized Data)
      │
      ▼
Gold Layer (Business-Ready Analytics)
      │
      ▼
Microsoft Fabric Pipeline
      │
      ▼
Power BI Dashboard
```

---

# 🛠 Technologies Used

## Cloud Platform
- Microsoft Fabric
- OneLake
- Fabric Lakehouse

## Data Engineering
- PySpark
- Spark SQL
- Delta Lake
- Microsoft Fabric Notebooks

## Data Processing
- Data Cleaning
- Data Transformation
- Data Aggregation
- Data Validation
- Data Standardization

## Data Orchestration
- Microsoft Fabric Pipelines

## Data Visualization
- Power BI

## Programming Language
- Python
- SQL

## Version Control
- Git
- GitHub

---

# Project Structure

```
Enterprise-Healthcare-Analytics-Platform-on-Microsoft-Fabric/

│
├── 01_Bronze_Ingestion.ipynb
├── 02_Silver_Transformation.ipynb
├── 03_Gold_Transformation.ipynb
├── README.md
└── LICENSE
```

---

# 📁 Dataset

The project uses publicly available healthcare datasets containing:

- Hospital General Information
- Provider Services
- Unplanned Hospital Visits

These datasets are ingested into Microsoft Fabric Lakehouse and processed through Bronze, Silver, and Gold layers.

---

# 🥉 Bronze Layer

The Bronze layer stores raw healthcare data exactly as received.

### Tasks Performed

- Loaded CSV files into Microsoft Fabric
- Created Bronze Delta Tables
- Preserved original schema
- Stored raw data in OneLake

Tables Created

- bronze_hospital_information
- bronze_provider_services
- bronze_unplanned_hospital_visits

---

# 🥈 Silver Layer

The Silver layer performs data cleansing and transformation.

### Tasks Performed

- Removed duplicate records
- Standardized column names
- Trimmed whitespace
- Handled missing values
- Converted data types
- Applied business rules
- Created cleaned Delta tables

Output Table

- hospital_silver

---

# 🥇 Gold Layer

The Gold layer creates business-ready analytical datasets.

### Gold Tables Created

- gold_birth_friendly
- gold_emergency_services
- gold_hospital_ownership
- gold_hospital_type
- gold_state_summary
- gold_top_hospitals

These tables are optimized for reporting and dashboard creation.

---

# 🔄 Data Pipeline

The entire ETL process is orchestrated using Microsoft Fabric Pipelines.

Pipeline Execution Order

```
Bronze Ingestion
        │
        ▼
Silver Transformation
        │
        ▼
Gold Transformation
```

Each notebook executes sequentially to ensure data consistency throughout the Medallion Architecture.

---

# 📊 Power BI Dashboard

Power BI connects directly to the Gold Layer to provide business insights.

Dashboard includes:

- Hospital Overview
- State-wise Hospital Distribution
- Top Rated Hospitals
- Emergency Services Analysis
- Birth Friendly Hospitals
- Hospital Ownership Analysis

---

# 🧰 Skills Demonstrated

- Microsoft Fabric
- OneLake
- Fabric Lakehouse
- Microsoft Fabric Pipelines
- PySpark
- Spark SQL
- Delta Lake
- ETL Pipeline Development
- Medallion Architecture
- Data Cleaning
- Data Transformation
- Data Engineering
- Data Modeling
- Data Analytics
- Power BI
- Git
- GitHub

---

# 🚀 Project Workflow

```
CSV Files
      │
      ▼
OneLake
      │
      ▼
Bronze Notebook
      │
      ▼
Bronze Delta Tables
      │
      ▼
Silver Notebook
      │
      ▼
Silver Delta Table
      │
      ▼
Gold Notebook
      │
      ▼
Gold Delta Tables
      │
      ▼
Microsoft Fabric Pipeline
      │
      ▼
Power BI Dashboard
```

---

# 📈 Key Features

- End-to-End Data Engineering Project
- Microsoft Fabric Implementation
- Medallion Architecture
- Delta Lake Storage
- PySpark Data Processing
- Fabric Pipeline Orchestration
- Business-Ready Gold Layer
- Interactive Power BI Reporting
- Reproducible Notebook-Based Workflow

---

# 👨‍💻 Author

**Moulya Reddygari Bhupal**

- LinkedIn: https://www.linkedin.com/in/moulyarb/
- GitHub: https://github.com/Moulya002

---

## ⭐ If you found this project helpful, consider giving it a star!
