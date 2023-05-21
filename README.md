# TwitterSentimentAnalysis

Steps involved in this project:

Data collection - Created own dataset by extracting tweets from Twitter using Twitter API. Tweepy was used to regularly extract the tweets. All the tweets are stored in a csv file. A total of 2099 tweets were collected.

Data labelling - First, the tweets were cleaned by tokenizing and remove punctuations, stop words, user mentions, URLs, etc. Then, tweets were labelled according to their sentiment scores (1.0: Positive, 0.0: Neutral, -1.0: Negative). The sentiment scores were found using TextBlob. The csv file was updated to have a new column called 'Sentiment' which had the sentiment score corresponding to each tweet. The pie chart in 'Data Labelling' section shows the distribution of sentiments in the data.

Text Analytics - At first, the data had to be split into 80% training set and 20% test set. The text processing technique was applied again, this time including a normalization like Lemmatization. After this, the data was represented in different ways - Bag of words, Binary representation and TF-IDF. Three classifiers - Logistic Regression, Support Vector Machine (SVM) and Naive Bayes were evaluated on the TF-IDF vectorized data. The SVM classifier turned out to be the best classifier as it had a better F1-score (meaning, better perfomance across all classes). The graph under the 'Evaluation and comparison of classifiers' shows the result.

Visualization - Useful insights and graphs are shown.
