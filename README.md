# Amazon_Vine_Analysis

### Overview of the analysis: Explain the purpose of this analysis.
The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. We will need to analyze Amazon reviews written by members of the paid Amazon Vine program.

In this project, we choose one specific dataset named `amazon_reviews_us_Video_Games_v1_00.tsv.gz` from 50 datasets. Then we use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, we use PySpark to determine if there is any bias toward favorable reviews from Vine members in your dataset.

### Results: Using bulleted lists and images of DataFrames as support, address the following questions:

How many Vine reviews and non-Vine reviews were there?
How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

### Summary: In your summary, state if there is any positivity bias for reviews in the Vine program. Use the results of your analysis to support your statement. Then, provide one additional analysis that you could do with the dataset to support your statement.
