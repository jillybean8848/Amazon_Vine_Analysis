# Amazon_Vine_Analysis
***Amazon Vine Review Program Analysis using Pyspark, AWS, PostgreSQL and Pandas***

## Overview
In this project, we were supplied with approximately 50 datasets containing reviews of a specific program within The Amazon Vine program. The Amazon Vine Program is a service that allows manufacturers and publishers to receive reviews for their products. Companies can pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. For my analysis I choose to focus on the "Beauty" category. I enabled the use of PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Lastly, using Pandas, I determined if there was any bias toward favorable reviews from Vine members in the "Beauty" dataset. 

## Results
The Amazon Vines "Beauty" dataset was first read in with 5,115,666 reviews. In order to focus on the most effective reviews the dataset was filtered by:
   * Count of Total Votes equal or greater than 20.
  * Percent of Helpful Votes to Total Votes equal or greater than 50%.


 ### Total Vine/Non-Vine Reviews
 The previous filters helped to bring our total reviews focus down to 74,760. 
  * 647 Vine (paid) reviews
  * 74113 non Vine (unpaid) reviews
 ![total_reviews_count](https://user-images.githubusercontent.com/110632671/207783619-7d1d0137-5b9e-452e-b59f-5d6f51142a31.png)
 
 ### Total Five Star Vine/Non-Vine Reviews 
  * 228 five star Vine (paid) reviews
  * 42612 five star non_Vine(unpaid) reviews
 ![five_star_reviews](https://user-images.githubusercontent.com/110632671/207787560-6cfc3bd8-678a-40c0-b761-dcaa6d9cc0f0.png)
 
 ### Percentage of Five Star Vine/Non-Vine Reviews
  * 35% of five star reviews were paid Vine program reviews
  * 57% of five star reviews were not paid or part of the Vine program
  ![percentage_reviews](https://user-images.githubusercontent.com/110632671/207788112-46b8ee65-5562-4fcb-b141-d46777bfbcd8.png)

 

 

