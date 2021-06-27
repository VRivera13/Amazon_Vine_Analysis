# Amazon_Vine_Analysis

## Overview of the analysis:
A random data set from amazon reviews for music was selected.   I used Pyspark for hte ETL process to extrac data, transform the data and connect to the database within pgAdmin that I generated via the AWS webserver.    Goal objective is to determine if there is any bias with regards to favorable reviews from Vine members.

## Results:
- How many Vine reviews and non-Vine reviews were there?
    - There are a total of 7 vine reviews and 105,979 non-vine reviews in the dataset.
![total reivews](https://github.com/VRivera13/Amazon_Vine_Analysis/blob/main/images/Vine%20vs%20NonVine%20Reviews.PNG)

- How many Vine reviews were 5 stars?  How many non-Vine reviews were 5 stars?
    - 5 Star Vine Reviews: 0
    - 5 Star Non-Vine Reviews: 67580

![5 star reviews](https://github.com/VRivera13/Amazon_Vine_Analysis/blob/main/images/5%20stars.png)

- What percentage of Vine reviews were 5 stars?  What percentage of non-Vine reviews were 5 stars?
    - 0% of the 5 star reviews were Vine
    - 100% of the 5 star reviews were non-Vine.


## Summary
Based on the current data, there is no evidence of positivity bias for the reviews in the Vine program.    The results show that out of 105,986 reviews there were 67,580 5 stars reviews that were ALL from Non-Vine members.   Also to support no evidence of positivity bias, the percentages for both paid and unpaid reviews were within a margin of 3%, with paid reviews totaling 66.8% and unpaid reviews totaling 63.2%.    Not a huge variance to result in positivity bias.   An additional analysis that could also be suggested is to review the remaining 38,406 reviews that are less than 5 stars.    Majority of the less than 5 star reviews, would most likley have been given by Non-Vine members based on the current data.   It would be interesting to see how many were verified purchases.
