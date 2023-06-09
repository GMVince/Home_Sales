# Home_Sales
![sales_robot](/images/home_sales_robot_2.jpg)




## Instructions
Rename the Home_Sales_starter_code.ipynb file as Home_Sales.ipynb.

Import the necessary PySpark SQL functions for this assignment.

Read the home_sales_revised.csv data in the starter code into a Spark DataFrame.

Create a temporary table called home_sales.

Answer the following questions using SparkSQL:

## What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.

![4-bedroom-houses](/images/avg_4bdrm.png)

## What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off your answer to two decimal places.

![3-bedroom-houses](/images/avg_3bdrm.png)

## What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.

![neural](/images/avg_2k_sqr_ft.png)

## What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.

![ratings](/images/avg_350K.png)

![time](/images/avg_350k_time.png)

## Cache your temporary table home_sales.

## Check if your temporary table is cached.

## Using the cached data, run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.

![avg_cache](/images/avg_350k_cache.png)

![cache_time](/images/avg_350k_cache_time.png)

## Partition by the "date_built" field on the formatted parquet home sales data.

## Create a temporary table for the parquet data.

## Run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.

![avg_p](/images/avg_350k_parquet.png)

![time_p](/images/avg_350k_parquet_time.png)

## Uncache the home_sales temporary table.

## Verify that the home_sales temporary table is uncached using PySpark.

![racw](/images/check_cache_status.png)

# Conclusion:

The cached dataset ran faster at 0.696 seconds than the regular dataframe at 0.855 seconds.  The parquet dataframe was the slowest to process at 1.05 seconds

![time](/images/race_to_finish.jpg)


## References
Data for this dataset was generated by edX Boot Camps LLC, and is intended for educational purposes only.
Stack Overflow for schema data conversion - https://stackoverflow.com/questions/60646254/cannot-resolve-column-due-to-data-type-mismatch-pyspark
syntax with ChatGPT - https://chat.openai.com/
microsoft bing for images - https://www.bing.com/images/create/robot-searching-home-sales-data-and-houses/647684c8dfe648018e98b407610aff05?id=5h5v4xPfF%2BW04YBShmmDuw%3D%3D&view=detailv2&idpp=genimg&form=GCRIDP&ajaxhist=0&ajaxserp=0

© 2023 edX Boot Camps LLC
