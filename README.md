
# retail_analysis_on_databricks

# Technology Used
<img src='https://github.com/DuncanMPlate/retail_analysis_on_databricks/blob/main/Apache_Spark_logo.png?raw=true' height='100px'>
<img src='https://github.com/DuncanMPlate/retail_analysis_on_databricks/blob/main/databricks-logo.jpg?raw=true?raw=true' height='100px'>

This project is developed with (databricks)[https://databricks.com/] and (Apache Spark)[https://spark.apache.org/]

# Project Goals

* Create a list of all countries to which orders have been shipped.

* How many orders have been placed in total?

* How many orders have been shipped to each country?

* For each product, list its product ID, product name, and the company name.

* Which 5 countries have the heaviest shipments, on average?

* Which 10 companies have placed the most orders? List the contact name of each company.

* Sort the customers by total amount spent on orders in descending order.

* Sort customers with a total spending greater than 20,000 in descending order.

* Sort the employees by the number of orders they sold in descending order.

* How many employees account for about half of the orders? (You do not have to use SQL to answer this question. A rough estimate is sufficient.)

* List customers who have never placed an order.

* List the products with the highest level of discount in descending order.

# Observed Northwind ERD 
<img src='https://github.com/DuncanMPlate/retail_analysis_on_databricks/blob/main/ERD.png?raw=true' height='100px'>
after we read in the csv files, we analysed the ERD and observed how the data was connected. Orders felt to be a keystone table, with it's joinings connecting the rest of the database to itself. 

# Analysis Performed

* Using aggregation on the orders table we identified that there have been 830 orders placed

* Germany and the US have the most orders shipped 
<img src='https://github.com/DuncanMPlate/retail_analysis_on_databricks/blob/main/orders_by_country.png?raw=true' height='200px'>

* Austria, Ireland, USA, Germany, and Sweden are the countries with the heaviest orders 
<img src='https://github.com/DuncanMPlate/retail_analysis_on_databricks/blob/main/freight_by_country.png?raw=true' height='200px'>

* The top 10 companies placing orders and their contact information can be viewed here 
<img src='https://github.com/DuncanMPlate/retail_analysis_on_databricks/blob/main/companies_by_orders.png?raw=true' height='200px'>

* Customers by total spending 
<img src='https://github.com/DuncanMPlate/retail_analysis_on_databricks/blob/main/total_spending_by_company.png?raw=true' height='200px'>

# Data Attribution
Data Used in This Analysis is Provided by 2U. You can acquire the data using below links: 
* s3://2u-data-curriculum-team/dataviz-classroom/v1.1/22-big-data/categories.csv
* s3://2u-data-curriculum-team/dataviz-classroom/v1.1/22-big-data/customers.csv
* s3://2u-data-curriculum-team/dataviz-classroom/v1.1/22-big-data/employee-territories.csv
* s3://2u-data-curriculum-team/dataviz-classroom/v1.1/22-big-data/employees.csv
* s3://2u-data-curriculum-team/dataviz-classroom/v1.1/22-big-data/order-details.csv
* s3://2u-data-curriculum-team/dataviz-classroom/v1.1/22-big-data/orders.csv
* s3://2u-data-curriculum-team/dataviz-classroom/v1.1/22-big-data/products.csv
* s3://2u-data-curriculum-team/dataviz-classroom/v1.1/22-big-data/regions.csv
* s3://2u-data-curriculum-team/dataviz-classroom/v1.1/22-big-data/shippers.csv
* s3://2u-data-curriculum-team/dataviz-classroom/v1.1/22-big-data/suppliers.csv
* s3://2u-data-curriculum-team/dataviz-classroom/v1.1/22-big-data/territories.csv
