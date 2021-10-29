# AirlineTweetClassification

# Introduction
This project is used to classify tweets from various users tweeted on their experience with US airlines - US Airways, United, American, Southwest, Delta, and Virgin America. Various sentiments of the tweets weere classified into Positive, Negative and Neutral. The classification of these tweets were done using a deep learning model _'Bidirectional LSTM (Long-Short Term Memory)-CNN (Convolutional Neural Networks) with Attention Mechanism'_ . The main aim of this project was to understand the deep learning model using a toy dataset and how it can be used for sentiment analysis or topic classification applications.

# Dataset
The data set used is from Kaggle- [Dataset]<br>

Columns:



- text: The actual tweet
- airline: Name of the airline tweeted about
- latitude, longitude: Location of the tweet
- airline_sentiment_confidence : Confidence of the sentiment classification of the tweet
- airline_sentiment: Sentiment of the tweet



Composition of the sentiments of the tweet:



- negative    9178
- neutral     3099
- positive    2363

# Model

- Embedding layer:
The words given as input in the input layer needs to be converted into a vector representation. The words are mapped to a corresponding real value vector that contains the syntatic and semantic meaning of the words. Pre-trained GloVe was used for creating the matrix.

- Bidirectional Recurrent Layer:
RNN maintains the sequential information of the input. The variable length sequences are mapped to fixed length vectors by truncating the sequences. For the purpose of this project LSTM was used because it can avoid vanishing gradient problem. LSTM can control the flow of information using gates that decide to remove, add or keep information.

# Data Insights
[Insights]


[Dataset]: https://www.kaggle.com/crowdflower/twitter-airline-sentiment
[Insights]: https://github.com/anjaliasha123/AirlineTweetClassification/blob/main/src/DataInsights.ipynb
