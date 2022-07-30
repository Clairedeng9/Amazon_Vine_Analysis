# Amazon_Vine_Analysis

### Overview of the analysis: Explain the purpose of this analysis.
The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. We will need to analyze Amazon reviews written by members of the paid Amazon Vine program.

In this project, we choose one specific dataset named `amazon_reviews_us_Video_Games_v1_00.tsv.gz` from 50 datasets. Then we use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, we use PySpark to determine if there is any bias toward favorable reviews from Vine members in your dataset.

### Results: Using bulleted lists and images of DataFrames as support, address the following questions:

![image](https://user-images.githubusercontent.com/103073631/181878773-ca82142b-35c5-4142-84b9-3908ad4c42b7.png)

From above to answer below questions:
How many Vine reviews and non-Vine reviews were there?
- Total vine reviews are 94;
- Total non-vine reviews are 40471.

How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
- There 48 vine reviews were 5 stars, and 15663 non-vine reviews were 5 stars.

What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
- The percentage of vine reviews were 5 stars is `51.06%`; and the percentage of non-vine reviewers were 5 stars is `38.70%`

### Summary: In your summary, state if there is any positivity bias for reviews in the Vine program. Use the results of your analysis to support your statement. Then, provide one additional analysis that you could do with the dataset to support your statement.

- From the percentage of Vine reviews or non-Vine reviews, the 51.06% from vine reviews is greater than 38.70% from non-Vine reviews, which indicates that positive bias toward favorable reviews from Vine members in the dataset. However, the total vine reviews are only 94, comparing with the non vine reviews are 40,471, the volumn of vine reviews are far smaller than the volumn of non vine reviews. It is too early to say there is a positive bias, aggresively saying, there is a positive bias.

- For additional analysis that I would do with the dataset is to approve if it is statistically significant, we will have a set of two samples hypothesis tests, H0 will be the mean percentages of vine reviews and non vine reviews are equal; H1 will be the mean of percentages of vine reviews is greater than the mean of percentages of non vine reviews.
