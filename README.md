Amazon Alexa Reviews (Twitter Sentiment Analysis)

Overview
This project focuses on sentiment analysis of tweets related to Amazon Alexa, using a dataset obtained from Kaggle. The goal is to classify tweets as either positive or negative using Natural Language Processing (NLP) techniques and machine learning algorithms. 

Data Source: https://www.kaggle.com/datasets/sid321axn/amazon-alexa-reviews

Dataset: Amazon Alexa Reviews from Kaggle

Project Steps
1. Import Libraries and Load Dataset
   
Necessary libraries such as pandas, numpy, seaborn, matplotlib, and jupyterthemes are imported. The dataset is loaded into a DataFrame named tweets_df, with initial data exploration performed using .info() and .describe().

3. Data Exploration
   
Exploratory Data Analysis (EDA) is conducted, including:

Visualizing missing data using a heatmap.
Plotting histograms and count plots for data distribution and label counts.
Calculating the length of each tweet and visualizing its distribution.

3. Word Cloud Generation
Word clouds are generated for the entire dataset, as well as for positive and negative tweets, to visualize the most frequent words.

4. Data Cleaning
Data cleaning involves:

Removing punctuation and stopwords from the tweets using string and nltk libraries.
Implementing a custom function message_cleaning() for preprocessing text.
5. Count Vectorization (Tokenization)
The cleaned data is vectorized using CountVectorizer to convert text data into numerical format, suitable for model training.

6. Model Training and Evaluation
A Naive Bayes classifier is trained on the processed data:

Data is split into training and test sets.
The model is evaluated using a confusion matrix and classification report, providing metrics like precision, recall, and F1-score.
Conclusion
The project successfully demonstrates sentiment analysis using NLP techniques and a Naive Bayes classifier. The model achieves high accuracy, especially in identifying positive tweets.

Future Work
Future improvements could include exploring more advanced models like LSTM or BERT for better sentiment classification.
