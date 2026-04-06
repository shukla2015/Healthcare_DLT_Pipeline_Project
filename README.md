# Healthcare Delta Live Tables (DLT) Pipeline

This project demonstrates a **medallion architecture pipeline** for healthcare data using **Databricks Delta Live Tables (DLT)**. Raw healthcare records are ingested, validated, and transformed through Bronze, Silver, and Gold layers.

## 🔧 Tech Stack
- Databricks Delta Live Tables (DLT)
- PySpark / Python
- Delta Lake
- Azure Data Lake Storage Gen2

## 📁 Notebooks Overview

| Notebook | Description |
|---|---|
| `feed_raw_tables` | Simulates raw data ingestion into Bronze layer |
| `healthcare_dlt_processing` | DLT pipeline — applies quality checks and builds Silver/Gold tables |

## 📌 Key Concepts Covered
- Delta Live Tables pipeline definition
- Medallion Architecture (Bronze → Silver → Gold)
- Built-in data quality constraints (`@dlt.expect`)
- Automated pipeline orchestration via Databricks Workflows

## 🔄 Architecture
Raw Data → Bronze (feed_raw_tables) → Silver (validated) → Gold (aggregated analytics)

## 🚀 How to Run
1. Import both notebooks into your Databricks workspace.
2. Create a new **Delta Live Tables pipeline** and attach `healthcare_dlt_processing` notebook.
3. Run `feed_raw_tables` first to populate raw data.
4. Trigger the DLT pipeline to process data end-to-end.

## 👤 Author
Shashank Shukla — [GitHub](https://github.com/shukla2015)
