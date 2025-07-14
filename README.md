# Procurement Data Engine

A modular, production-style procurement analytics platform designed to handle SaaS product purchases, vendor service contracts, and ad hoc service requests — powered by a normalized relational schema and AWS-based ETL pipelines.

---

## 📌 Project Overview

This project documents the **end-to-end architecture** and **data pipeline design** for a procurement platform built around structured client-vendor-product relationships. It focuses on clean **data modeling**, **Excel-based ingestion**, and **ETL orchestration** using AWS services such as S3, Glue, and RDS.

The ultimate goal is to build a foundation for future **visual analytics dashboards** (e.g., QuickSight) and **AI chatbot interfaces** that can query and summarize procurement intelligence.

---

## 🚀 Key Features

- 📦 **Header–Detail schema** for contracts, invoices, and service requests  
- 🧠 Step-by-step normalization from unstructured Excel to 3NF  
- ⚙️ AWS-first ETL pipeline (Excel → S3 → Glue → RDS)  
- 🧾 Support for one-time service requests & long-term vendor contracts  
- 📊 Ready for dashboarding, forecasting, and AI extensions

---

## 🧱 Tech Stack

| Layer       | Tools Used                                   |
|-------------|-----------------------------------------------|
| Data Storage | Amazon S3 (raw + cleansed zones)              |
| Processing   | AWS Glue (PySpark-based transformation)       |
| Database     | Amazon RDS (PostgreSQL)                       |
| Analytics    | Amazon Athena, QuickSight (planned)           |
| Modeling     | dbdiagram.io / MySQL Workbench (EER design)   |
| Source Upload | Excel templates (user uploads)               |

---

## 📁 Repository Structure

```text
/procurement-data-engine/
├── README.md
├── LICENSE
├── docs/
│   ├── 01_data-modeling/
│   │   ├── 1.1_raw_schema.xlsx
│   │   ├── 1.2_normalization_steps.md
│   │   ├── 1.3_final_normalized_schema.md
│   │   ├── 1.4_EER_diagram.png
│   │   └── 1.5_table_descriptions.md
│   └── 02_etl-design/
│       ├── 2.1_s3_folder_structure.md
│       ├── 2.2_etl_flow_diagram.png
│       ├── 2.3_glue_script_sample.py
│       ├── 2.4_rds_schema.sql
│       └── 2.5_data_validation_rules.md
├── schema/
│   ├── ddl/
│   │   ├── clients.sql
│   │   ├── service_requests.sql
│   │   └── ...
│   └── dbml/
│       └── schema.dbml
---

## 📖 Documentation Highlights

- 📄 **1.2_normalization_steps.md** – Step-by-step breakdown of converting unstructured data into 1NF, 2NF, and 3NF  
- 🗃️ **1.3_final_normalized_schema.md** – Fully normalized schema with header–detail structures  
- 🧭 **1.4_EER_diagram.png** – Entity-relationship diagram reflecting final table design  
- 🧪 **2.5_data_validation_rules.md** – Transformation and validation logic applied during ETL  
- 🔁 **2.2_etl_flow_diagram.png** – Visual representation of S3 → Glue → RDS data flow

---

## 🔭 Future Scope

- 📊 Amazon QuickSight dashboards for spend analysis, vendor performance, and SLA tracking  
- 🤖 AI chatbot integration (RAG-based) to answer contract, invoice, or service request questions  
- 🌐 Optional UI/API layer for Excel uploads, validation, and trigger management

---

## 🧑‍💻 Author

**Medhavi**  
Data Engineering & Analytics Enthusiast | Passionate about building scalable data platforms

---
