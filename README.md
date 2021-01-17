# Amazon Vine Analysis

## Overview of Analysis

The purpose of this analysis was to determine if there might be any bias for a five star review when the review is left by a paid
Vine member of Amazon, versus a regular shopper of the product.  The data set I performed analysis on was provided by Amazon and
were reviews left only for watches.  This was the only data set I analyzed out of the roughly forty that were provided. I used pySpark
and jupyter notebooks through Google Colab to ETL the data to my cloud based RDS (PostgresSQL) provided by Amazon. Then I extracted the
data from Postgres and used the Pandas library in a jupyter notebook to run my analysis.

## Results
To make the results of my analysis look cleaner, I created a summary dataframe to showcase the differences between vine reviews
and non-vine reviews.

![alt text](https://github.com/jseverin1984/Amazon_Vine_Analysis/blob/main/Resources/summary%20dataframe.png "summary dataframe")

- How many Vine reviews and non-Vine reviews were there?

	There were 47 total vine reviews.
	There were 8362 total non-vine reviews.

- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

	There were 15 five star vine reviews.
	There were 4332 five star non-vine reviews.

- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

	Of the total vine reviews, only 31.91% were five star reviews.
	Of the total non-vine reviews, 51.81% were five star reviews.

# Summary

Based off of the single data set I analyzed, there showed no bias in favor of five star reviews written by paid Amazon Vine members.
In this data set, a non-vine reviewer was 1.6 times more likely to leave a five star review for a purchased watch than the paid Vine member.
I was only tasked with finding how many five star reviews were left when trying to find any bias towards favorable reviews. This does
not paint a full picture.  Further analysis is needed to find a more accurate answer. Such as grouping four and five star reviews as
positive and then calculating the percentage against the total number of reviews.  This may or may not change the answer to whether or
not a paid Vine member shows a bias to writing a more favorable review than regular customers.





