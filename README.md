# Amazon_Vine_Analysis

## Overview
We set out to determine if Vine members were more likely to provide positive reviews in exchange for free products. To test this we created a database using AWS, SQL and colabs that allowed us to filter through Amazon user review data. We looked at the data to see if reviewers in the Vine program, exhibit bias in their product reviews. For background, the Vine program was or is one in which, if I understand correctly, companies pay Amazon and provide Vine members with products at no cost in exchange for product reviews. The results...may surprise you.

## Results
Nope. Are reviewers promiscuous with 5-star reviews when there is SWAG involved? Probably not. I didn't do any stats on it, but the percentage of 5-star reviews is about the same, as you'll see. (This is a work in progress.)

We wrote pyspark code in colab to filter through massive amounts of data in order to learn the answers to three questions:

### QUESTION ONE
  - How many Vine reviews were there? How many non-Vine reviews?
  
  
### QUESTION TWO
  - How many Vine reviews were 5-star reviews? How many non-Vine reviews?


### QUESTION THREE 
  - What percentage of of each category were 5-star reviews?

#### Percentage of 5-star Vine reviews
<img width="604" alt="Screen Shot 2022-04-20 at 12 05 57 AM" src="https://user-images.githubusercontent.com/4724180/164154392-865e8466-8782-4249-825a-e298782cdaf7.png">

#### Percentage of 5-star non-Vine reviews
<img width="642" alt="Screen Shot 2022-04-20 at 12 08 23 AM" src="https://user-images.githubusercontent.com/4724180/164154619-4233b726-d7e1-4fda-a0aa-cdebe8324d75.png">

## Summary
As we see from those percentages, the likelyhood of getting a 5-star review on Amazon seems unlikely to be dependent on participation in the Vine program. More likely, it appears, good products will get good reviews.

One way to learn more about how likely it is that Amazon reviews are unbiased would be apply some statistical rigor to the question. We could also just check the frequency of 1-star reviews.
