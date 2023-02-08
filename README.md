# Amazon Vine Analysis

## Overview 
The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.
In this project, we will have access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. I have picked the amazon reviews for US video games and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, you’ll use PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in your dataset. 

Deliverable 1: Perform ETL on Amazon Product Reviews
Deliverable 2: Determine Bias of Vine Reviews

Software Used :
 Google Colaboratory, Pyspark, AWS RDS , Postgres, 
 
## Results: 

  - Creation of Spark DataFrame

    The entire dataset recorded 1,785,997 number of rows in the dataset.


  ## 1.1 Creation of customers_table DataFrame
  TODO : - image

  ## 1.2 Creation of products_table DataFrame
   TODO : -image
 
  ## 1.3 Creation of review_id table DataFrame

  TODO : - image

  ## 1.4 Creation of Vine_table DataFrame

  TODO : - image


    
## Deliverable 2 Results

 - How many Vine reviews and non-Vine reviews were there?
 
    - There were 94 vine reviews .

    - There were 40,471 non-vine reviews
    - Total reviews (vine + non-vine) = 94 + 40,471 = 40,565 reviews

    Of these the vine reviews constitute only 0.23% of the total
    ( 94/40,565 ) * 100 = 0.23%

    Non-vine total percentage :
     (40,471 / 40,565) * 100 = 99.8%



 - How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
    - There were 48 5-star vine reviews
    - There were 15,663 5-star non-vine reviews


 - What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
    - Percentage of 5-star reviews of  vine program is 51.0638%
    - Percentage of 5-star reviews of non-vine program is 38.7018%


 ## Summary:

  In your summary, state if there is any positivity bias for reviews in the Vine program. Use the results of your analysis to support your statement. Then, provide one additional analysis that you could do with the dataset to support your statement.
 
 Based on the results, vine members did not show much bias towards the rating of the products due to the below reasons

  - Although , the percentage of the 5-star reivews in vine program (51.06%)  is more than the percentage of non-vine program, the total population of the non-vine reviews much more (99%) comapared of the 1% of the vine population.

  -  Only 51% of the entire vine reviewers gave 5-star ratings and not all of the vine reviewers gave 5-star ratings

  These results were based of the video games datasets and we would have to also comapre the results among other data-sets to come to a final conculsion to check whether there is any bias or non-bias. 
