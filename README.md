# Amazon_Vine_Analysis
***Amazon Vine Review Program Analyis using Pyspark, AWS, PostgreSQL and Pandas***

## Overview
In this project, we were supplied with approximately 50 datasets containing reviews of a specific program within The Amazon Vine program. The Amazon Vine Program is a service that allows manufacturers and publishers to receive reviews for their products. Companies can pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. For my analysis I choose to focus on the "Beauty" category. I enabled the use of PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Lastly, using Pandas, I determined if there was any bias toward favorable reviews from Vine members in the "Beauty" dataset. 

## Results
The Amazon Vines "Beauty" dataset was first read in with 5,115,666 reviews. In order to focus on the most effective reviews the dataset was filtered by:
   * Count of Total Votes equal or greater than 20.
  * Percent of Helpful Votes to Total Votes equal or greater than 50%.


 ### How many74113 Vine reviews and non Vine reviews were there?
 The previous filters helped to bring our total reviews focus down to 74,760. 
  * 647 Vine (paid) Reviews
  * 74113 non Vine (unpaid) reviews
 ![total_reviews_count](https://user-images.githubusercontent.com/110632671/207783619-7d1d0137-5b9e-452e-b59f-5d6f51142a31.png)

 

