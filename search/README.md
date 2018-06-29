# Search query datasets

## Overview
There are over 900,000 unique words extracted from search queries. These words were labeled by algorithm and judges for word segmentation task. Our segmentation criteria is to segment the longest food word as possible for archiving the highest precision score in search system.

## Files
+ `labeled_query_by_algo.txt` : List of 900K words labeled by algorithms which were described in detail in this [blog.]( https://life.wongnai.com/wongnai-search-improvement-using-machine-learning-part1-e0777b65979e)

+ `labeled_query_by_judges.txt` : List of 10K words labeled by judges following Wongnai's search criteria.

+ `food_dictionary.txt` : List of 400K food words used for labelling the labeled_query_by_algo file.

**Please note that these words were collected from user-generated content(UGC) which might include some out of topic words.**

## How to use
- You may use `labeled_query_by_algo.txt` for training your own word segmentation model by spliting into train and validation set and then evaluate your model with `labeled_query_by_judges.txt`


