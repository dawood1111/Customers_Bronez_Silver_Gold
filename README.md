# Customers ETL Pipeline: Databricks + Orchestration

An end-to-end data engineering project that ingests a customers dataset (2,000,000 rows), cleans it, builds business-ready tables, runs automatically every day, and visualizes the results in Power BI.

## Business Scenario

A company receives customer data as files and wants to:
1. Load the raw data automatically, without manual work.
2. Clean it and apply business rules.
3. Answer questions about subscriptions (per year, per country).
4. See the results in a dashboard that stays up to date.

## Tech Stack

- Databricks (Unity Catalog, Lakeflow Declarative Pipelines, Jobs)
- PySpark / Python
- Medallion architecture (Bronze, Silver, Gold)
- Power BI

## Pipeline and Job

Pipeline 
<img width="929" height="830" alt="Screenshot 2026-11-13 211037" src="https://github.com/user-attachments/assets/111206c2-248c-493f-994e-14146050b3f5" />

Job
<img width="1343" height="856" alt="Orchestration" src="https://github.com/user-attachments/assets/2b368f33-5c37-4496-8b0f-e05fc76dac8e" />

## Author
`dawood adel dawood jaber` 
