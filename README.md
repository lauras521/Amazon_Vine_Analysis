# Amazon Vine Analysis for Sports Data

## Overview

### Purpose
The purpose of this project is to use knowledge of PySpark and Pandas to determine if there is any bias towards product reviews in the Amazon Vine program.  Vine reviews are paid reviews and non-vine reviews are unpaid reviews.  

## Analysis and Results

### Analysis
Data was gathered on the sports Amazon dataset.  PySpark and Google Colab were used to read in the dataset.  4 unique tables were created:
1. customers table
2. products table
3. review id table
4. vine table

Amazon Web Services were used to host a database and connect to PGAdmin to be able to load these tables into a SQL database .  The vine table was further manipulated in Google Colab using PySpark and Pandas and the results are below. 

### Results
* How many vine reviews and non-vine reviews were there?
    * vine reviews: 334
    * non-vine reviews: 61,614
* How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
    * 5 star vine reviews: 139
    * 5 star non-vine reviews: 32,665
* What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
    * percentage of 5 star vine reviews: 42%
    * percentage of 5 star non-vine reviews: 53%

See image below for a summary of the data above:
<p align="center">
  <img src = https://github.com/lauras521/Amazon_Vine_Analysis/blob/8288ba2f5032e0c5f9250b9cf6d276e6e027cd89/Resources/deliverable_2_results_image.PNG>
</p>

### Summary
By further manipulating the vine table I wanted to determine if there is any positive bias in the vine program (i.e. does paying for reviews sway the reviewers rating higher than not paying for reviews).  There are significantly fewer vine reviews than non-vine reviews (334 vs. 61,614).  The percentage of 5 star reviews is actually lower in the vine program than the non-vine program so there does not appear to be any positivity bias.  For additional analysis you could breakout reviews further looking at overall positive (i.e. 4 and 5 stars), overall negative (i.e. 1 and 2 stars), and overall neutral (i.e. 3 stars) reviews.  You could also run statistical tests to strengthen your conclusion about bias. 


## Resources
[link to Amazon Product Reviews Database](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt)

[link to code](https://github.com/lauras521/Amazon_Vine_Analysis/blob/8288ba2f5032e0c5f9250b9cf6d276e6e027cd89/Vine_Review_Analysis.ipynb)
