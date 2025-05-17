# 🛍️ RetailRadar Pipeline

**RetailRadar Pipeline** is a robust data engineering project that simulates a real-world retail analytics backend. It processes **point-of-sale (POS)** data from multiple sources (CSV, JSON), performs data cleaning and transformation, and enables insightful retail analytics such as **top-selling products**, **seasonal trends**, and **stockout risk detection**.

The pipeline uses **dbt** for modular data modeling and **Apache Airflow** for orchestration and scheduling. It serves as a foundation for a retail analytics dashboard.


## 📌 Features

- 📥 **Data Ingestion**:
  - Reads and unifies POS data from CSV and JSON formats
  - Supports batch processing of sales, inventory, and product metadata

- 🧹 **Data Cleaning & Transformation**:
  - Handles nulls, duplicates, and inconsistent data types
  - Standardizes timestamps, product IDs, and category fields

- 🏗 **Data Modeling with dbt**:
  - Dimensional modeling (fact_sales, dim_product, dim_store)
  - Incremental builds and source freshness checks
  - Derived metrics: sales volume, revenue, stock status

- 📈 **Analytics & Insights**:
  - Top-selling products by region and category
  - Weekly/monthly trend analysis
  - Stockout detection based on inventory vs. sales velocity

- 📆 **Orchestration with Airflow**:
  - DAGs to schedule ingestion, transformation, and reporting tasks
  - Task failure alerts and logging for pipeline monitoring


## 🛠️ Tech Stack

- **Data Processing**: Python, Pandas
- **Data Modeling**: dbt (Data Build Tool)
- **Workflow Orchestration**: Apache Airflow
- **Storage**: PostgreSQL or Snowflake (configurable)
- **Visualization**: Ready for integration with dashboards (e.g., Metabase, Tableau)



## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- PostgreSQL (or another supported warehouse)
- dbt Core
- Apache Airflow (via Docker or local install)

### Clone & Install

```bash
git clone https://github.com/your-username/retail-radar-pipeline.git
cd retail-radar-pipeline
pip install -r requirements.txt
