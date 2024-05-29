# Home Sales Analysis with SparkSQL
# Module 22 Challenge

In this challenge, you'll use your knowledge of SparkSQL to determine key metrics about home sales data. The tasks involve creating temporary views, partitioning data, caching and uncaching a temporary table, and verifying the caching status.

## Project Structure

- [Home_Sales.ipynb](https://github.com/myhre062/Home_Sales/blob/main/Home_Sales.ipynb): The Jupyter Notebook containing the complete code for the challenge.

## Tasks

1. **Setup Spark and Java Environment**
   - Install necessary packages and set up the environment for running Spark.
   - Initialize a Spark session.

2. **Data Ingestion**
   - Read the home sales data from an AWS S3 bucket into a Spark DataFrame.

3. **Data Processing and Analysis**
   - Create a temporary view from the DataFrame.
   - Execute various SQL queries to calculate key metrics:
     - Average price for a four-bedroom house sold per year.
     - Average price of homes built each year with 3 bedrooms and 3 bathrooms.
     - Average price of homes built each year with 3 bedrooms, 3 bathrooms, two floors, and a minimum of 2,000 square feet.
     - Average price of homes per "view" rating, with an average price greater than or equal to $350,000.

4. **Caching**
   - Cache the temporary view and verify that it is cached.
   - Run a query using the cached data and compare the runtime to the uncached runtime.

5. **Partitioning**
   - Partition the home sales data by the `date_built` field and save it as Parquet files.
   - Read the partitioned Parquet data and create a temporary view from it.
   - Run a query using the Parquet data and compare the runtime to the cached runtime.

6. **Uncaching**
   - Uncache the temporary view and verify that it has been uncached.

## How to Run

1. Ensure you have a suitable environment for running Spark, such as Google Colab or a local setup with Jupyter Notebook.
2. Open [Home_Sales.ipynb](https://github.com/myhre062/Home_Sales/blob/main/Home_Sales.ipynb) in your environment.
3. Follow the notebook cells sequentially to execute the tasks.

## Key Points

- The project demonstrates the use of SparkSQL for performing data analysis on home sales data.
- It highlights the benefits of caching and partitioning in Spark to optimize query performance.
- The project ensures that the temporary tables are properly managed, including caching and uncaching operations.

## Conclusion

This challenge provides hands-on experience with SparkSQL, showcasing its capabilities for big data processing and analysis. By following the tasks outlined, you will gain a deeper understanding of how to leverage Spark for efficient data management and querying.
