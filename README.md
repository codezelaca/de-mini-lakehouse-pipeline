# Mini Lakehouse Pipeline Demo

## Project Purpose

This project is a student-friendly demonstration of a mini data engineering pipeline using free tools. It is built to explain and show the data engineering workflow, not to serve as a real production system.

This repository was created for a course practical to demonstrate the following concepts:

- environment setup for PySpark and Delta Lake
- raw data ingestion from CSV files
- conversion to Parquet for storage optimization
- Delta Lake table creation for ACID metadata and versioning
- Time Travel queries to read older dataset versions
- a simple Spark Structured Streaming example

> This is a learning exercise. It demonstrates concepts used in data engineering pipelines, rather than a production-ready application.

## What is included

- `end_to_end_lakehouse_pipeline (1).ipynb` — the main notebook with the full pipeline walkthrough.
- `ecommerce_sales_34500.csv` — the sample raw dataset used for ingestion.

## Key Concepts Covered

1. Environment setup with PySpark and Delta Lake.
2. Loading raw CSV data into Spark.
3. Inspecting schema and sample rows.
4. Writing data to Parquet for optimized analytics.
5. Creating a Delta Lake table and using Delta transaction logs.
6. Demonstrating Delta Lake Time Travel to query previous table versions.
7. Introducing Spark Structured Streaming with a simple live stream example.

## How to run this project

### Option 1: Open in Google Colab

1. Open `end_to_end_lakehouse_pipeline (1).ipynb` in Google Colab.
2. Run the first cells to install dependencies:
   - `!pip install pyspark`
   - `!pip install delta-spark`
3. Run the notebook cells in order.

### Option 2: Run locally in Jupyter

1. Install Python if not already installed.
2. Install required packages:
   - `pip install pyspark`
   - `pip install delta-spark`
3. Open the notebook in Jupyter and execute cells sequentially.

## Notebook Flow

The notebook demonstrates a complete mini lakehouse pipeline step-by-step:

- Setup the Spark environment with Delta Lake support.
- Load `ecommerce_sales_34500.csv` as a Spark DataFrame.
- Examine the raw data and schema.
- Save the cleaned dataset as Parquet.
- Read Parquet back and compare performance.
- Save the dataset as a Delta table.
- Update the Delta table to create a new version.
- Query an earlier version of the Delta table using Time Travel.
- Run a small Spark Structured Streaming demo.

## Why this matters

Even though this project is a demonstration, the concepts are important for modern data engineering:

- Parquet is used for fast, columnar analytics.
- Delta Lake adds reliability, metadata, and version control on top of data lakes.
- Time Travel helps with auditability and recovering previous data states.
- Streaming introduces how data can be processed continuously.

## Notes for course grading

- This is a course practical that brings together the pipeline topics taught in class.
- The notebook is designed to be educational and easy to follow.
- It is not a production data platform.

## File summary

- `end_to_end_lakehouse_pipeline (1).ipynb` — core notebook walkthrough.
- `ecommerce_sales_34500.csv` — sample dataset.

If you want, I can also add a short “how to present this project” section or a simplified task checklist for exam/demo use." 


### github repo link - https://github.com/codezelaca/de-mini-lakehouse-pipeline
