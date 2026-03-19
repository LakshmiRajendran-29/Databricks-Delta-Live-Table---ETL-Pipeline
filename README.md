Project Title 

Databricks Lakehouse Delta Live Tables (DLT) ETL Pipeline – Medallion Architecture

Production-style Databricks ETL pipeline Lakehouse using Delta Live Tables with Medallion Architecture.

⚙️ Spark Declarative Pipelines (SDP) – Processing Engine

This project uses Spark Declarative Pipelines (Delta Live Tables) to simplify pipeline development and management.

🔄 Automatic Orchestration

	•	No need to manually define execution order
	•	The system automatically:
	•	Builds a DAG (Directed Acyclic Graph)
	•	Executes transformations in the correct sequence

⚡ Incremental Processing

	Uses:
	•	Streaming Tables
	•	Materialized Views
	•	Processes only new or changed data, instead of full reloads
	•	Improves:
	•	Performance
	•	Cost efficiency

🛡️ Built-in Data Quality

	•	Data quality rules (expectations) are defined directly in the pipeline

	Supports:
	
	•	Dropping invalid records
	•	Alerting on failures
	•	Quarantining bad data

🔀 Unified Batch & Streaming
	•	Same pipeline supports:
	•	Real-time streaming
	•	Batch processing
	•	Eliminates need for separate architectures


🚀 Key Highlights

	•	End-to-end ETL pipeline using Databricks
	•	Scalable Medallion Architecture implementation
	•	Automated pipeline orchestration using DLT
	•	Incremental data processing for efficiency
	•	Built-in data quality enforcement

📖 Project Overview

This project demonstrates a modern data engineering pipeline built using Databricks, Spark Declarative Pipelines (SDP), and the Medallion Architecture.

The pipeline is designed to:

	•	Ingest raw data from source systems
	•	Apply data validation and transformation
	•	Deliver curated, business-ready datasets

🏗️ Architecture

Bronze Layer → Raw ingestion (Streaming Tables)
       ↓
Silver Layer → Cleaned & transformed data
       ↓
Gold Layer → Aggregated business-ready data


🔄 Pipeline Flow

🟫 Bronze Layer (Raw Data Ingestion)

	•	Acts as the landing zone for incoming data
	•	Stores data as-is from source systems
	•	Minimal transformation applied
	•	Serves as a historical archive for reprocessing

	•	bronze_addresses
	•	bronze_customers
	•	bronze_orders

👉 Features:

	•	Streaming ingestion
	•	Raw data storage
	•	Schema applied

🟩 Silver Layer (Data Cleaning & Transformation)

	Data is cleaned, filtered, and transformed

	Provides an enterprise-level view of core entities such as:

	•	silver_addresses
	•	silver_customers
	•	silver_orders
	•	silver_orders_clean

	Used for:
	
	•	Ad-hoc reporting
	•	Data science workloads

Transformations:

	•	Data cleansing
	•	Deduplication
	•	Standardization
	•	Business rule validation

🟨 Gold Layer (Business Aggregation)

	•	Contains aggregated and enriched datasets
	
Optimized for:
	
	•	Business intelligence
	•	Dashboards
	•	Analytical queries
	•	Example:
	•	Customer order summary
	•	KPI metrics

👉 Features:

	•	Aggregated data
	•	Ready for reporting & analytics

⚙️ Technologies Used

	•	Databricks Delta Live Tables (DLT)
	•	Apache Spark (PySpark)
	•	Delta Lake
	•	Structured Streaming
	•	Medallion Architecture

🧠 Key Concepts Demonstrated

Example:

📊 Pipeline DAG

<img width="1642" height="1196" alt="image" src="https://github.com/user-attachments/assets/67f98a86-5740-4e3f-8a30-f8fdafd1fb44" />

🚀 How to Run
	1.	Create a DLT pipeline in Databricks
	2.	Upload notebooks to workspace
	3.	Configure pipeline settings
	4.	Run pipeline (Development / Production mode)

📌 Key Learnings
	•	Handling streaming data pipelines in Databricks
	•	Optimizing ETL workflows using DLT
	•	Designing scalable data architectures
	•	Understanding pipeline orchestration

🔥 Future Enhancements
	•	Add data quality expectations (DLT expectations)
	•	Implement CDC (Change Data Capture)
	•	Add monitoring & alerting
	•	Optimize performance using partitioning & Z-order

This project demonstrates how modern data platforms like Databricks enable building scalable, reliable, and maintainable data pipelines with minimal operational overhead using Declarative Pipelines and Medallion Architecture.

Lakshmi Rajendran
Data Engineer | Spark | Databricks | AWS
