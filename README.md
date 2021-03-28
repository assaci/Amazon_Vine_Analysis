# Amazon_Vine_Analysis

"SellBy pays a fee to Amazon to use one of their services "Amazon Vine Program" which allows companies to provide products to Amazon Vine members, in return, they receive feedback for the products."
The goal of this project was to analyze the Amazon Vine program and provided a report to SellBy stakeholders if there was any positivity bias for reviews in the Vine program. 
In this study, we used PySpark to perform ETL on Amazon Product Reviews and determine the Bias of Vine Reviews.

# Results

## Perform ETL on Amazon Product Reviews

For my analysis, I choose Home_Improvement reviews from Amazon Reviews dataset. I created an AWS RDS database with tables in pgAdmin. I used Google Colab Notebook to extract the Home_Improvement data and created  4 DataFrames :the customers_table DataFrame, products_table DataFrame, review_id_table DataFrame and vine_table DataFrame.

![Cust](https://github.com/assaci/Pyber_Analysis/blob/main/pict/Cust.PNG?raw=true)

![Prod](https://github.com/assaci/Pyber_Analysis/blob/main/pict/Prod.PNG?raw=true)

![review](https://github.com/assaci/Pyber_Analysis/blob/main/pict/review.PNG?raw=true)

![vine](https://github.com/assaci/Pyber_Analysis/blob/main/pict/vine.PNG?raw=true)

## Determine Bias of Vine Reviews


