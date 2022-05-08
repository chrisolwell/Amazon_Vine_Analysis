# Amazon_Vine_Analysis

## Overview
We set out to determine if Vine members were more likely to provide positive reviews in exchange for free products. To test this we created a database using AWS, SQL and colabs that allowed us to filter through Amazon user review data. We looked at the data to see if reviewers in the Vine program, exhibit bias in their product reviews. For background, the Vine program was or is one in which, if I understand correctly, companies pay Amazon and provide Vine members with products at no cost in exchange for product reviews. The results...may surprise you?

## Results
It depends what you expected. Are reviewers loose with 5-star reviews when there is free stuff involved? Probably not. I didn't do any stats on it, but the percentage of 5-star reviews is about the same, as you'll see. 

We wrote pyspark code in colab to filter through massive amounts of data in order to learn the answers to three questions:

### QUESTION ONE
  - How many Vine reviews were there? How many non-Vine reviews?

  #### Non-Vine reviews
  <img width="642" alt="Screen Shot 2022-04-20 at 12 28 00 AM" src="https://user-images.githubusercontent.com/4724180/164156821-b029d06a-84b8-4b77-972e-1b0b4bb3467c.png">
  
  #### Vine reviews
  <img width="642" alt="Screen Shot 2022-04-20 at 12 29 08 AM" src="https://user-images.githubusercontent.com/4724180/164156924-825f0ab9-a05c-4940-8c50-ef5d62da02eb.png">

### QUESTION TWO
  - How many Vine reviews were 5-star reviews? How many non-Vine reviews?

  #### Vine 5-star reviews
  <img width="642" alt="Screen Shot 2022-04-20 at 12 30 15 AM" src="https://user-images.githubusercontent.com/4724180/164157034-22e10b15-2073-45a9-951d-04725ec0031f.png">
  
  #### Non-Vine 5-star reviews
  <img width="642" alt="Screen Shot 2022-04-20 at 12 32 00 AM" src="https://user-images.githubusercontent.com/4724180/164157229-048ac02a-4279-4c08-b6a2-d6d553c40cc8.png">


### QUESTION THREE 
  - What percentage of of each category were 5-star reviews?

#### Percentage of 5-star Vine reviews
<img width="604" alt="Screen Shot 2022-04-20 at 12 05 57 AM" src="https://user-images.githubusercontent.com/4724180/164154392-865e8466-8782-4249-825a-e298782cdaf7.png">

#### Percentage of 5-star non-Vine reviews
<img width="642" alt="Screen Shot 2022-04-20 at 12 08 23 AM" src="https://user-images.githubusercontent.com/4724180/164154619-4233b726-d7e1-4fda-a0aa-cdebe8324d75.png">

## Summary
As we see from those percentages, the likelyhood of getting a 5-star review on Amazon seems unlikely to be dependent on participation in the Vine program. More likely, it appears, good products will get good reviews.

One way to learn more about how likely it is that Amazon reviews are unbiased would be apply some statistical rigor to the question. We could also check the frequency of 1-star reviews across the same two categories and see if there's much variance there.
