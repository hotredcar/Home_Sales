# Home_Sales Analysis 

## Introduction
In this project, we utilized SparkSQL to analyze key metrics about home sales data. Our tasks included creating temporary views, partitioning the data, caching and uncaching a temporary table, and verifying the cache status.

## Data Overview
We started by reading the home_sales_revised.csv data into a Spark DataFrame and created a temporary table named home_sales to work with.

## Key Metrics Analysis
We answered several questions using SparkSQL:

* Average Price for Four-Bedroom Houses: We calculated the average price for a four-bedroom house sold for each year.
* Average Price of Homes by Built Year and Bedrooms/Bathrooms: We determined the average price of homes for each year they were built, considering specific criteria such as bedrooms and bathrooms.
* Average Price of Homes by Built Year and Specific Features: We analyzed the average price of homes for each year they were built, considering additional features like floors and square footage.
* Average Price of Homes per "View" Rating: We calculated the average price of homes per "view" rating, considering only homes with an average price greater than or equal to $350,000. We also determined the runtime for this query.

## Temporary Table Cache
We cached the temporary table home_sales and verified its cache status. We then ran a query on the cached table and compared its runtime with the uncached runtime. Afterward, we uncached the table.

## Partitioning Parquet Data
We partitioned the home sales dataset by the "date_built" field and read the formatted parquet data. We created a temporary table for the parquet data and ran the same query as before, comparing the runtime with the uncached runtime.

## Conclusion
Throughout this project, we demonstrated our proficiency in utilizing SparkSQL to analyze and derive insights from large datasets. By leveraging Spark's capabilities, we efficiently processed and analyzed home sales data, providing valuable insights for further analysis.