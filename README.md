# Amazon_Vine_Analysis

"SellBy pays a fee to Amazon to use one of their services "Amazon Vine Program" which allows companies to provide products to Amazon Vine members, in return, they receive feedback for the products."
The goal of this project was to analyze the Amazon Vine program and provided a report to SellBy stakeholders if there was any positivity bias for reviews in the Vine program. 
In this study, we used PySpark to perform ETL on Amazon Product Reviews and determine the Bias of Vine Reviews.

# Results

## Perform ETL on Amazon Product Reviews

For this analysis, I choose Home_Improvement reviews from Amazon Reviews dataset. I created an AWS RDS database with tables in pgAdmin. I used Google Colab Notebook to extract the Home_Improvement data and created  4 DataFrames :the customers_table DataFrame, products_table DataFrame, review_id_table DataFrame and vine_table DataFrame.

![Cust](https://github.com/assaci/Amazon_Vine_Analysis/blob/main/pict/Cust.PNG?raw=true)

![Prod](https://github.com/assaci/Amazon_Vine_Analysis/blob/main/pict/Prod.PNG?raw=true)

![review](https://github.com/assaci/Amazon_Vine_Analysis/blob/main/pict/review.PNG?raw=true)

![vine](https://github.com/assaci/Amazon_Vine_Analysis/blob/main/pict/vine.PNG?raw=true)

## Determine Bias of Vine Reviews

For this analysis, to determine if having a paid Vine review would make a difference in the percentage of 5-star reviews, i filtered vine_table data and calculated the total number of reviews, the number of 5-star reviews, and the percentage of 5-star reviews for the two types of review (paid vs unpaid):

![perc](https://github.com/assaci/Amazon_Vine_Analysis/blob/main/pict/perc.PNG?raw=true)

- total paid reviews 26573
- total unpaid reviews 12522
- total number of reviews  39095
- total 5-star reviews 18371
- Percentage of 5-star reviews 47%
- Percentage 5-star reviews are calculated for all Vine reviews 49%
- Percentage 5-star reviews are calculated for non Vine reviews 41%



## Summary 

From the findings, SellBy received a total of 39095 reviews. From these reviews, 26573  as 68% reviews were from Amazon Vine Program and 12522 as 32% were from nonVine program. 
The number of 5-star reviews was 18371 as 47% of all Vine and nonVine reviews.
From the number of 5-star reviews, 49% were from the Vine program and 41% were from the nonVine program. 
Even if the percentage of paid and unpaid reviews were slightly different (8%), They were both in the 40% range. 
In conclusion, there was no positivity bias for reviews in the Vine program. 



