# Wongnai-corpus
This project is a collection of Wongnai's datasets which are mostly in Thai language. We hope that these datasets will advance Thai natural language processing(NLP) research.

## 1. Search query dataset
There are 500,000 unique words extracted from search queries. These words were labeled by algorithm and judges for a word segmentation task. Our segmentation criteria is to segment the longest food word as possible for archiving the highest precision score in search system.

### 1.1 Files
+ `search/labeled_query_by_algo.txt` : List of 500K words labeled by algorithms which were described in detail in this [blog post.]( https://life.wongnai.com/wongnai-search-improvement-using-machine-learning-part1-e0777b65979e)

+ `search/labeled_query_by_judges.txt` : List of 10K words labeled by judges following Wongnai's search criteria.

+ `search/food_dictionary.txt` : List of 400K food words used for labelling the labeled_query_by_algo file.

**Please note that these words were collected from user-generated content(UGC) which might include some out of topic words.**

### 1.2 Usage
- You may use `labeled_query_by_algo.txt` for training your own word segmentation model by spliting into train and validation set and then evaluate your model with `labeled_query_by_judges.txt`.


## 2. Review dataset
The review dataset contains restaurant reviews and ratings (there are only 5 classes ranging from 1 to 5 stars).

### 2.1 Files
- The dataset is located in [Kaggle competition](https://www.kaggle.com/c/wongnai-challenge-review-rating-prediction) which was created by Aj.Ekapol Chuangsuwanich 

### 2.2 Usage
- The dataset is originally used for a Review Rating Prediction task. You can find an example of how to import the data from [this](https://colab.research.google.com/drive/1iOweEcd78oLdMAvAWOE6fNLp94aGv7th#scrollTo=8dihf3f3COtm).(by Khun Korakot Chaovavanich)

- In addition, it is also used for creating a [Text Classification Benchmark](https://github.com/kobkrit/nlp_thai_resources/blob/master/README.md). which was well described in [this](https://colab.research.google.com/drive/1cnJ6O3b1jwaHwvsMWW3oQw7f8X2Ka7Sp#scrollTo=jNTJ5rl6eKLB).(by Khun Charin Polpanumas)