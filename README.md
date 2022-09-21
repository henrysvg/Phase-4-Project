# Twitter Sentiment Analysis for Target


## Project Overview

This project uses tweets which have been assigned an emotion to build a machine learning model that can be utilized as a tool by Target to understand which products they show showcase or put on sale during the upcoming holiday season.


## Business Problem

Target is one of the world largest retailers with a big electornic department in most stores. As the holiday season is approaching large retail sellers like Target are beginning to focus on what should be showcased in their stores especially during times where sales occur.  Target is looking to better understand the sentiment behind the products which they are selling in their electornics department.  By building a model that can use twitter data from one of the worlds largest technology conferences they will better understand what is looked upon positively and what is looked upon negatively from potential buyers.


## The Data

The dataset comes from CrowdFlower via data.world. Human Raters rated the sentiment in over 9,000 Tweets as positive, negative, or neither (neutral). The dataset shows that this twitter set was most likely pulled from those who were attending the SXSW conference due to the amount of mentions in the tweets.


## Word Cloud of Emotion Behind Tweet


### Positive Word Cloud

![Postive_Word_Cloud.png](./Images/Positive_Word_Cloud.png)

### Negative Word Cloud

![Negative_Word_Cloud.png](./Images/Negative_Word_Cloud.png)

### Neutral Word Cloud

![Neutral_Word_Cloud.png](./Images/Neutral_Word_Cloud.png)


## NLP

Natural Langauge Processing was utilized to clean the twitter data.  This process included:
* Standardizing
* Tokeninzing

After cleaning the text data, you could look at frequency of words in the full dataset:

### Word Frequency

![Frequency.png](./Images/Frequency.png)


## Modeling Process

Three different models were created before choosing the best fit model.  Before modeling was done, the data was vectorized using TF-IDF Vecotrizer.

### Model Types:
* Basekline Model with Multinomial NB
* Random Forest
* XGBoost

## Conclusion

The best fit model was XGBoost utlizing best parameters.  This model will acurately predict the emotion of a tweet 68% of the time.  Neutral was the best predicted emotion due to it having the most tweets.  It is reccomended to utilize this model to predict the emotion behind specific products which will be sold at target.  It is also recommended to utilize this model with more data to increase the scores.