# Amazon_Vine_Analysis

## Overview of Analysis

This analysis analyzes a dataset of Amazon reviews of sport products written by members of the paid  Amazon Vine program. PySpark is used to perform the ETL process, extract the dataset, transform the data,  conneect to an AWS RDS instance, then load the transformed data into pgAdmin. The data is also analyzed to determine if having a paid Vine Review makes a difference in the percentage of of 5 star reviews. 

### Results
* Number of Vine reviews

+----------------+
|count(review_id)|
+----------------+
|             334|
+----------------+

* Number of Non-Vine reviews

+----------------+
|count(review_id)|
+----------------+
|           61614|
+----------------+

* Five Star Vine Reviews 

Result: 139

* Five Star Non-Vine Reviews

 > Result: 32665

* Percentage of Vine Reviews Five stars

 > Result: 42%

* Pecentage of non-Vine Five stars

 > Result: 53%


#### Summary

Based on the result of 42% of five stars for paid Vine reviews and 53% five stars for non-paid Vine reviews, there does not seem to be a bias in the review of the prodcuts. An additional analysis can be perfomed analyzing the review_headline column using Natural language proccessing to analyze the text data to further support this statement.