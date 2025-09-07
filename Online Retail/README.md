## Overview



Analysis of the UCI Online Retail dataset (https://archive.ics.uci.edu/dataset/352/online+retail), which contains over 500,000 transactions from a UK-based online store between 2010–2011. The dataset includes invoices, products, customer IDs, quantities, prices, and countries.



#### Project Goals:



* Clean and preprocess raw transaction data 
* Analyze sales performance using SQL queries (DuckDB in Python)  
* Visualize trends, top products, and customer behavior  
* Derive actionable business insights



#### Key Steps:



* Data Cleaning -Removed duplicates and invalid records (negative quantities, missing values)
* Converted date columns to datetime
* Standardized product descriptions and customer IDs
* SQL Analysis
* Basic queries: COUNT, SUM, AVG, DISTINCT
* Advanced queries: window functions, ranking, monthly trends, top customers
* Visualizations
* Line charts for revenue trends
* Bar charts for top products and top customers
* Stacked bar charts for country-level revenue



#### • Key Insights:



* Revenue peaks in December, indicating seasonal trends
* A small set of top products drives most of the revenue
* Top customers contribute disproportionately to total sales
* UK dominates revenue, but other European countries show meaningful sales



**Tech Stack:** Python, Pandas, DuckDB, Matplotlib, Seaborn

