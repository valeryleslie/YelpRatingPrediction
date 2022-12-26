# Yelp Rating Prediction - NLP

A Yelp dataset consisting of Californian restaurants is analysed to create a predictive algorithm.

# Data Cleaning

Transferred the five-star rating system into a binary system Good (4-5 Stars) and Bad (1-3 Stars).
Mutated the "Elite" column into a numeric number of years a user is considered an Elite member. 

## Natural Language Processing - Sentiment Analysis on Review Text
- Removed special characters including punctuations, tabs, backslashes and redundant white spaces
- Removed stop words using the removeWords function in R
- Performed word stemming on each word using stemDocument- Porter's stemming algorithm

### Mutations:
- Bing Sentiment Lexicon: Column additions of number of positive words, number of negative words, and sentiment of positive - negative words
- Affin Sentiment Lexicon: Column additions of total 'point' of sentiment in the review and normalization of total 'point' divided by number of words in each cleaned review (Affin rates each word on a -5 to +5 point)

# Predictive Algorithms

## Correlation Matrix

Correlation Matrix shows multicollinearity- will need PCA dimension reduction to produce a better predictive algorithm

![alt text](https://github.com/valeryleslie/YelpRatingPrediction/blob/main/CorrelationMatrix.png)

After PCA, multicollinearity is reduced.

![alt text](https://github.com/valeryleslie/YelpRatingPrediction/blob/main/CorrMatrixPCA.png)

## Algorithms Performed

- Naive Bayes 
- Multinomial Logistic Regression
- Support Vector Machine
- Random Forests

# Accuracy Table for each algorithm

![alt text](https://github.com/valeryleslie/YelpRatingPrediction/blob/main/Accuracy-Table.png)

