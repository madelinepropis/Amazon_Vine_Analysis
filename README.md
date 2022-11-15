# Amazon_Vine_Analysis

## Overview of the Analysis
The purpose of this analysis was to use PySpark to perform an ETL process on Amazon reviews written by members of the paid Amazon Vine program. This program allows members to post reviews for manufacturers and publishers to see. The Amazon Vine members are required to publish a review for the products they buy. I chose to extract the beauty dataset. I then transformed this data in PySpark. Lastly, I determined if there was any bias toward favorable reviews from Vine members in the dataset using Pandas.

## Results

### Vine Reviews

As shown in the above table, there are 647 total Vine reviews and 74,113 total non-Vine reviews.

### 5-Star Vine Reviews

As shown in the above table, there are 229 Vine 5-star reviews and 43,217 5-star non-Vine reviews.

### Percentage of 5-Star Vine Reviews

The percentage of 5-star Vine reviews is 35.39% and the percentage of 5-star non-Vine reviews is 58.31%.

## Summary
Based on the results, it appears that there is not positivity bias for reviews in the Vine program. The percentage of 5-Star reviews for Vine members is smaller than that of non-Vine members. It seems that when people are forced to review a product, they tend to rate it lower. This discrepency can also be attributed to non-Vine members more frequently reviewing products positively, and not reviewing products negatively as often.

Another analysis that I would do with this dataset is checking the star ratings with only verified purchases. It is possible that people are rating products that they did not even purchase. If the review has a verified purchase tag along with it, it should be counted, but if not, it should be excluded to reduce any potential errors. 