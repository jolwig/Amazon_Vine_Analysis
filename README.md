# Amazon_Vine_Analysis

##Overview
For this project, I analyzed Amazon reviews for video games. Some of the reviews were written by members of the paid Amazon Vine program and some were not. I wanted to determine if there is a bias between paid and non paid reviews. I extracted and cleaned the data using Google colab and pyspark and I used pandas to analyze the data. 

##Results
The dataset contained 6 columns:
"review_id" - Unique ID for each review
"star_rating" - Product rating on a scale of 1-5
"helpful_votes" - Number of Amazon users that voted a review as being helpful
"total_votes" - total number of review votes
"vine" - Tells if the review was a part of the Amazon Vine program or not
"verified_purchase" - Tells if the review was made buy someone who has proven they purchased the product

Here are some of the findings:
<img width="478" alt="image" src="https://user-images.githubusercontent.com/79022140/230255536-c90d48e4-bea6-488b-b1ce-b47badf46b6c.png">



The first thing I did during my analysis was remove all reviews that did not have more than 20 total_votes. The reasoning behind this was that reviews with more 

##Summary
