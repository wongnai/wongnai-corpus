# Wongnai-corpus
This project is a collection of Wongnai's datasets which are mostly in Thai language. We hope that these datasets will advance research in natural language processing(NLP) especially in Thai language.

## 1. Search query dataset
There are 500,000 unique words extracted from search queries. These words were labeled by algorithms and judges for a word segmentation task. Our segmentation criteria is to segment the longest food word as possible for archiving the highest precision score in search system.

### 1.1 Files
+ `search/labeled_queries_by_algo.txt` : List of 500K words labeled by algorithms which were described in detail in [blog post.]( https://life.wongnai.com/wongnai-search-improvement-using-machine-learning-part1-e0777b65979e)

+ `search/labeled_queries_by_judges.txt` : List of 10K words labeled by judges following Wongnai's search criteria.

+ `search/food_dictionary.txt` : List of 400K food words used for labelling the `labeled_queries_by_algo.txt`.

**Please note that these words were collected from user-generated content(UGC) which might include some out of topic words.**

### 1.2 Usage
- You may use `labeled_queries_by_algo.txt` for training your own word segmentation model by spliting into train and validation set and then evaluate your model with `labeled_queries_by_judges.txt`.


## 2. Review dataset
The review dataset contains restaurant reviews and ratings (there are only 5 classes ranging from 1 to 5 stars).

### 2.1 Files
- The dataset is located in [Kaggle competition](http://bit.ly/cu-2018-nlp) which was created by [Dr.Ekapol Chuangsuwanich](https://www.facebook.com/ekapolc) 

- If you can't download files, they are also located here `review/review_dataset.zip`

### 2.2 Usage
- The dataset is originally used for a Review Rating Prediction task. You can find an example of how to import the data from [here](https://colab.research.google.com/drive/1iOweEcd78oLdMAvAWOE6fNLp94aGv7th#scrollTo=8dihf3f3COtm). (by [Khun Korakot Chaovavanich](https://www.facebook.com/korakot.chaovavanich))

- In addition, it is also used for creating a [Text Classification Benchmark](https://github.com/PyThaiNLP/classification-benchmarks) which was well described [here](https://github.com/cstorm125/thai2fit/blob/master/wongnai_cls/classification.ipynb). (by [Khun Charin Polpanumas](https://www.github.com/cstorm125))


## Wongnai data services
- If you are interested in Wongnai database such as photos, reviews or restaurant database,
Wongnai also provides data services including API and files. For more details, please follow the link below.
https://business.wongnai.com/restaurants-data-service/en/

