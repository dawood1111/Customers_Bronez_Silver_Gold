# Customers ETL Pipeline: Databricks + Power BI

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

![Pipeline graph]

![Job runs](screenshots/job_runs.png)

## Project Structure

```
pipeline/    → bronze, silver, gold code
powerbi/     → dashboard file
screenshots/ → pipeline, job, and dashboard images
```

## How to Run

1. Import the `pipeline/` files into a Databricks pipeline.
2. Set the catalog and schema to `[your catalog.schema]`.
3. Run the pipeline, then schedule it as a Job.
4. Connect Power BI using the SQL warehouse's server hostname and HTTP path.

## Data Note

The dataset (2,000,000 customer records) is not included in this repo. Source: `[where you got it]`.

## Challenges and What I Learned

- Fixed a `SyntaxError` caused by wrong indentation in a pipeline function.
- Delta tables reject spaces in column names, so I added a snake_case rename step.
- `[add your own, such as the Power BI connection or the full refresh vs normal run]`

## Author

`[Your name]` | `[LinkedIn link]`
