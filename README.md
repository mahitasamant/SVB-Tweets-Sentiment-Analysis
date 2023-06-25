# SVB-Tweets-Sentiment-Analysis
This project focuses on performing sentiment analysis on a dataset of tweets related to the collapse of Silicon Valley. The goal is to analyze the sentiment expressed in these tweets using the K-nearest neighbors (KNN) algorithm and the VADER (Valence Aware Dictionary and sEntiment Reasoner) sentiment analysis tool.

Dataset
The dataset used in this project contains the following columns:

Unnamed: 0: Index column
date: Date and time of the tweet
id: Unique identifier for the tweet
tweet: Text of the tweet
username: Username of the tweet author
likecount: Number of likes received by the tweet
retweetcount: Number of retweets received by the tweet
Steps
Data Preprocessing: The tweet text is preprocessed to remove any noise, unwanted characters, or inconsistencies. This step ensures the data is clean and ready for sentiment analysis.

VADER Sentiment Analysis: The VADER sentiment analysis tool is used to calculate sentiment scores for each preprocessed tweet. VADER provides a compound score that represents the overall sentiment of a text.

Discrete Sentiment Labels: The sentiment scores are converted into discrete sentiment labels. A threshold value is chosen to classify the tweets as positive, negative, or neutral. Tweets with a compound score above the threshold are labeled as positive, those below the threshold are labeled as negative, and those close to the threshold are labeled as neutral.

Feature Extraction: The sentiment scores or labels are used as features for training the KNN classifier. Additional features such as 'likecount' and 'retweetcount' can also be considered. The data is prepared for training the classifier.

KNN Training: The KNN classifier is trained on the labeled data, with the sentiment scores or labels as the target variable. The number of neighbors (K) is specified, and the classifier learns to classify new, unlabeled tweets based on their similarity to the labeled data.

Sentiment Analysis of Unlabeled Data: The trained KNN classifier is used to predict the sentiment of unlabeled tweets related to the Silicon Valley collapse. These tweets can be from a different time period or dataset. The sentiment analysis provides insights into public opinion and sentiment trends surrounding the event.

# Getting Started
To run this project, follow these steps:

Clone the repository: gh repo clone mahitasamant/SVB-Tweets-Sentiment-Analysis


# Results and Analysis
The sentiment analysis results are provided in the form of labeled tweets and predictions for unlabeled tweets. These results can be further analyzed and visualized to gain insights into the sentiment trends related to the collapse of Silicon Valley.

# Conclusion
This project demonstrates the application of sentiment analysis using the KNN algorithm and the VADER sentiment analysis tool on a dataset of tweets related to the collapse of Silicon Valley. Training a KNN classifier can predict the sentiment of new, unlabeled tweets. The project provides a foundation for understanding public sentiment and opinion surrounding this event.


# Acknowledgements
Dataset=https://www.kaggle.com/datasets/xreyas/svb-crisis-tweets

