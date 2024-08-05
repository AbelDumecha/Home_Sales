# Home Sales Analysis with PySpark (Module_22 Challenge)

## Overview

In this challenge, using SparkSQL to analyze home sales data, I created temporary views, partition data, and manage caching and uncaching of tables.

## Steps

1. **Import Libraries and read the data:**
   - Import the necessary PySpark SQL functions.
   - Load `home_sales_revised.csv` into a Spark DataFrame.

2. **Create Temporary Table:**
   - Register the DataFrame as a temporary table named `home_sales`.

3. **Run Queries:**
   - Calculate average prices for:
     - Four-bedroom houses by year.
     - Homes built each year with three bedrooms and three bathrooms.
     - Homes meeting specific criteria (three bedrooms, three bathrooms, two floors, and ≥2000 sqft).
     - Homes per "view" rating with an average price ≥ $350,000.

4. **Cache the Table and compare the performance:**
   - Cache the `home_sales` table and verify caching.
   - Measure and compare the runtime of queries on cached and uncached tables.

5. **Partition, save the Data and create temporary table for Parquet:**
   - Partition the DataFrame by `date_built` and save it as Parquet.
   - Read the partitioned Parquet data into a new DataFrame and create a temporary table.
   
6. **Run and Compare Performance on Parquet Data:**
    - Measure and compare the runtime of queries on Parquet data.

7. **Uncache and Verify:**
    - Uncache the `home_sales` table and verify it is uncached.

8. **Upload to GitHub:**
    - Download the `Home_Sales.ipynb` file and upload it to your "Home_Sales" GitHub repository.