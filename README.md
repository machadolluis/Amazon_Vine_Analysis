# Amazon_Vine_Analysis

## Overview

This project focuses on analyzing the Amazon Vine program to determine if there is a bias towards positive reviews from Vine members in comparison to free users. The source comes from [Amazon Review datasets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt), and the chosen category for analysis was Digital Software Purchases. 
This analysis uses PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, load the transformed data into pgAdmin and calculate different metrics.

## Results

* Vine Reviews:

![](/images/total_paid_reviews)
![](/images/paid_star_reviews)
![](/images/paid_star_percent)
To avoid division by zero, a try/except statement was used to state that there are no Vine reviews on this specific dataset for Digital Software Purchases at Amazon.

* Non-Vine Reviews:

![](/images/total_unpaid_reviews)
![](/images/unpaid_star_reviews)
![](/images/unpaid_star_percent)

## Summary

The dataset shows no reviews from Vine members.
Though there were no Vine reviews written for any of the products, the non-Vine review percentage that had 5 stars is 14.9% - not showing a majorly positive view on the products. Analyzing the statistical distributions of the star ratings could provide more insight on the reviews. 
