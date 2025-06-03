# Sentiment-Analysis-of-stock-news
This project is based on evaluating the performance of ML models(SVM, Decision Tree, RNN, LSTM, CNN) and traditional method (using tf-idf scores and SentiWordNet) in performing sentiment analysis of stock news.

The data has been web scraped from finviz.com for 10 companies(Amazon, Google, Meta, Apple, Microsoft, Nike, McDonald's, Nvidia, P&G, Tesla).

After data collection, preprocessing is done, this includes stopword removal, lemmatization, punctuation removal, etc.

Labels are assigned to the data using NLTK's Sentiment Intensity Analyzer, these labels will be used as the ground truth for evaluation and for training the ML models.

For the tradtional approach, the tf-idf scores and the sentiment scores from SentiWordNet are multiplied for each word and the values of each word in a headline is added, based on this value the labels are assigned as positive or negative.

The aim is to develop a system that will generate sentiment analysis of the input stock based on real time news extracted from finviz at runtime.
