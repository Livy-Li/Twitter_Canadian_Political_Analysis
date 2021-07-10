# Twitter_Canadian_Political_Analysis
Natural Language Processing (NLP) - Sentiment Analysis

---
# Background and Datasets
The purpose of this project is to compute the sentiment of text information - in this case, tweets posted recently on Canadian Elections - and answer the research question: “What can public opinion on Twitter tell us about the Canadian political landscape in 2019?” The goal is to essentially use sentiment analysis on Twitter data to get insight into the Canadian Elections.

Two sets of data are used for this project. The sentiment_analysis.csv file contains generic tweets that have had their sentiments already analyzed and recorded as binary values 0 (negative) and 1 (positive). Each line is a single tweet, which may contain multiple sentences despite their brevity. The comma-separated fields of each line are:

|Column Index|Column Name|Column Content|
|---|---|---|
|0|ID|Tweet ID|
|1|text|the text of the tweet|
|2|label|the polarity of each tweet (0 = negative sentiment, 1 = positive sentiment)|

The second data set, Canadian_elections_2019.csv contains a list of tweets regarding the 2019 Canadian PM elections. The fields of each line are:

|Column Index|Column Name|Column Content|
|---|---|---|
|0|text|the text of the tweet|
|1|sentiment|can be “positive” or “negative”|
|2|negative_reason|reason for negative tweets. NaN for positive tweets|

Both datasets have been collected directly from the web, so they may contain html tags, hashtags, and user tags.

---

# Summary
The project is broken down into 6 different parts:
1. Text cleaning - include removing URL, html tags, special characters etc. for both datasets
2. Exploratory analysis - graphically present some aspects of both datasets
3. Training and testing 7 different classification models using the generic dataset - using two different types of features, Bag of Words and TF-IDF
4. Implementation the best model on the second dataset
5. Try to predict the "negative_reason" in the second dataset
6. Discussion of the research question
