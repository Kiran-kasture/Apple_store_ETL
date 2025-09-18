Apple Dataset ETL Pipeline



This project demonstrates a complete ETL (Extract, Transform, Load) workflow using Python, PySpark, PostgreSQL (Supabase), and Power BI.



📌 Workflow



Extract



faker generates synthetic Apple dataset (category, products, stores, sales, warranty).



Script appends new records every 2 days.



After 10 days, data resets to simulate rolling dataset.



Data saved in data/raw/ as CSV files.



Transform



PySpark script cleans the raw CSV files:



Handles nulls, duplicate records



Standardizes date formats



Ensures referential integrity (foreign keys)



Cleaned files saved in data/clean/.



Load



Cleaned data is uploaded into PostgreSQL (Supabase).



Tables: category, products, stores, sales, warranty.



Visualize



Power BI connects to Supabase.



Dashboards show:



Sales trends



Product category performance



Store-wise revenue



Warranty claim patterns



🛠️ Tech Stack



Python (Faker for data generation)



PySpark (Data cleaning/transformation)



PostgreSQL / Supabase (Data warehouse)



Power BI (Visualization)

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