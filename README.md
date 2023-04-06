# Amazon_Vine_Analysis

## Overview
For this project, I analyzed Amazon reviews for video games. Some of the reviews were written by members of the paid Amazon Vine program and some were not. I wanted to determine if there is a bias between paid and non paid reviews. I extracted and cleaned the data using Google colab and pyspark and I used pandas to analyze the data. 

## Results
The dataset contained 6 columns:
*"review_id" - Unique ID for each review
*"star_rating" - Product rating on a scale of 1-5
*"helpful_votes" - Number of Amazon users that voted a review as being helpful
*"total_votes" - total number of review votes
*"vine" - Tells if the review was a part of the Amazon Vine program or not
*"verified_purchase" - Tells if the review was made buy someone who has proven they purchased the product

Here are some of the findings from the original dataset:

<img width="478" alt="image" src="https://user-images.githubusercontent.com/79022140/230255536-c90d48e4-bea6-488b-b1ce-b47badf46b6c.png">

* A majority of the reviews are 5-star reviews
* Only a small portion of the total 5-star reviews were written by people in the Vine program

This data is not all that useful, so I created a new dataset that only contains the reviews that have more than 20 votes and more than 50% of the votes were "helpful votes". From the new dataset I created two more datasets; one that contains the reviews that were written by people in the Vine program and one that contains reviews written by people not in the Vine program. I also found the average star rating for the Vine and non-Vine datasets.

<img width="473" alt="image" src="https://user-images.githubusercontent.com/79022140/230260592-0c00b768-754a-4b5c-92f9-abd425eebb09.png">

* There are significantly more reviews written by people not in the Vine program
* Vine program reviews have a higher star rating

## Summary
Based on the average star ratings from the vine and non-vine datasets, vine reviewers might have a bias since they give much higher ratings. However, there are only 90 reviews in the vine dataset vs 37831 reviews in the non-vine dataset. We might see different results if the two datasets were closer to equal in size.
