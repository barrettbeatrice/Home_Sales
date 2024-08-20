# Home_Sales
This project uses SparkSQL to determine key metrics about home sales data. Spark was used to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached afterward.

Methodology:
  Import the necessary PySpark SQL functions and read csv data into Spark DataFrame.

  Create a temporary table called home_sales.

Use SparkSQL for insights (answers embedded in .ipynb code as Markdowns):

  What is the average price for a four-bedroom house sold for each year? 

  What is the average price of a home for each year the home was built, that has three bedrooms and three bathrooms?

  What is the average price of a home for each year the home was built, that has three bedrooms, three bathrooms, two floors, and    is greater than or equal to 2,000 square feet?

  What is the average price of a home per "view" rating having an average home price greater than or equal to $350,000? Note         the run time for this query.

Cache temporary table home_sales and check.

Using the cached data, run the last query that calculates the average price of a home per "view" rating having an average home price greater than or equal to $350,000. Compare this runtime to uncached runtime.

Partition by the "date_built" field on the formatted parquet home sales data.

Create a temporary table for the parquet data.

Run the last query that calculates the average price of a home per "view" rating having an average home price greater than or equal to $350,000. Compare runtime to uncached runtime.

Uncache the home_sales temporary table and verify with PySpark.
