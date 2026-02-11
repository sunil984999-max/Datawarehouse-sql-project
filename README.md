# 📊 SQL Data Warehouse Project: [Datawarehouse-sql-project]

## 📖 Project Overview
This project demonstrates the end-to-end development of a modern data warehouse using **SQL Server**. The goal is to consolidate disparate sales data from multiple source systems (e.g., ERP, CRM) into a single, unified source of truth for business intelligence and reporting.

### Key Features:
* **Medallion Architecture:** Implementation of Bronze (Raw), Silver (Cleaned), and Gold (Business) layers.
* **Automated ETL:** Stored procedures for automated data extraction, transformation, and loading.
* **Data Modeling:** Star Schema design featuring optimized Fact and Dimension tables.
* **Quality Assurance:** Integrated SQL scripts for data validation and integrity checks.

---

## 🏗️ Data Architecture
The project follows the **Medallion Architecture** to ensure data traceability and quality:

1.  **Bronze Layer (Raw):** Untouched data ingested directly from source CSV files. Used for traceability and debugging.
2.  **Silver Layer (Cleaned):** Standardized and deduplicated data. Includes data type casting, null handling, and business rule applications.
3.  **Gold Layer (Business):** Final analytics-ready layer. Uses views to present a Star Schema (Fact and Dimension tables) to BI tools.

---

## 🛠️ Technologies & Tools
* **Database Engine:** [SQL Server Express / (https://github.com/microsoft/sql-data-warehouse-samples)
* **IDE:** [SQL Server Management Studio (SSMS)](https://github.com/DataWithBaraa/sql-data-warehouse-project)
* **Modeling:** [Draw.io / Visio](https://github.com/gauravcx3/Data-Warehousing-Project) (for ER Diagrams)
* **Version Control:** Git & GitHub

---

## 📁 Project Structure
```text
├── datasets/           # Raw CSV source files
├── documents/          # Data Model & Architecture diagrams
├── scripts/
│   ├── init_db.sql     # Database & Schema initialization
│   ├── bronze/         # DDL and Load scripts for raw data
│   ├── silver/         # Transformation scripts for cleaning
│   └── gold/           # Views for Star Schema (Fact/Dims)
├── tests/              # SQL scripts for data quality checks
└── README.md
