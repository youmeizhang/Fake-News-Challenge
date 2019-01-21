# Fake News Stance Classification

This is a competition of MSCI 641 Text Analysis in University of Waterloo using the dataset from [Fake News Challenge](http://www.fakenewschallenge.org). The best model I built ranked Top 1 among 30 teams.

## 1D CNN
<img width="65%" height="65%" alt="example" src="https://github.com/youmeizhang/Fake-News-Challenge/blob/master/structures/1D-CNN.png">

## 2D CNN
<img width="65%" height="65%" alt="example" src="https://github.com/youmeizhang/Fake-News-Challenge/blob/master/structures/2D-CNN.png">

## GRU
<img width="65%" height="65%" alt="example" src="https://github.com/youmeizhang/Fake-News-Challenge/blob/master/structures/GRU.png">

## Model with Simple Attention
<img width="65%" height="65%" alt="example" src="https://github.com/youmeizhang/Fake-News-Challenge/blob/master/structures/SABi-GRU.png">

## Extra Features 
Extra features contribute to the improvement of the models and these features are:
* Sentiment
* Unigram, Bigram, Trigram ratio
* TF-IDF similarity
* Word2vec similarity

Below is a breif exploration of the influence using different extra features with simple classifiers. Based on this result, our models uses Ngram and TF-IDF similarity.

<img width="65%" height="65%" alt="example" src="https://github.com/youmeizhang/Fake-News-Challenge/blob/master/structures/Features%20Influence.png">


## Different Word Representation Methods
We also try to find the most suitable word representation for this specific task and we use Glove 300d in the competition.

<img width="65%" height="65%" alt="example" src="https://github.com/youmeizhang/Fake-News-Challenge/blob/master/structures/Different%20Vector%20Representation.png">

## Final Model Performance
1D CNN model performs the best in this case. However, please note that due to the long training process, these three models are all trained under 20 epoches and GRU is trained even with fewer epoches since it takes much time to train than the CNN models. It is possible that with more training epoches, these model might produce a better results.

<img width="65%" height="65%" alt="example" src="https://github.com/youmeizhang/Fake-News-Challenge/blob/master/structures/Model%20Performances.png">
