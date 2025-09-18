# Apple Store ETL Pipeline

This project demonstrates a complete ETL workflow using **Faker**, **PySpark**, **PostgreSQL (Supabase)**, and **Power BI**.

## Workflow
1. **Extract**: Generate synthetic Apple dataset with Faker (every 2 days, reset after 10 days).
2. **Transform**: Clean data using PySpark (handle nulls, duplicates, formats).
3. **Load**: Load cleaned data into PostgreSQL/Supabase.
4. **Visualize**: Build interactive dashboards in Power BI.

## Project Structure
Apple_store_ETL/
│── README.md
│── requirements.txt
│── notebooks/
│ ├── 01_data_extraction.ipynb
│ ├── 02_data_cleaning.ipynb
│ └── 03_data_analysis.ipynb
│── data/
│ ├── raw/
│ └── clean/
│── dashboard/
│ └── dashboard.pbix
