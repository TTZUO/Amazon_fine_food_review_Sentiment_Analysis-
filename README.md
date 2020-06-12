# Amazon fine food review Sentiment Analysis
 
This dataset consists of reviews of fine foods from amazon. The data span a period of more than 10 years, including all ~500,000 reviews up to October 2012. Reviews include product and user information, ratings, and a plain text review. It also includes reviews from all other Amazon categories.

Data includes:

Reviews from Oct 1999 - Oct 2012
568,454 reviews
256,059 users
74,258 products
260 users with > 50 reviews

attributes describe
1.Id
2.ProductId - unique identifier for the product
3.UserId - unqiue identifier for the user
4.ProfileName
5.HelpfulnessNumerator - number of users who found the review helpful
6.HelpfulnessDenominator - number of users who indicated whether they found the review helpful or not
7.Score - rating between 1 and 5
8.Time - timestamp for the review
9.Summary - brief summary of the review
10.Text - text of the review

https://www.kaggle.com/snap/amazon-fine-food-reviews

The purpose of this analysis is to make up a prediction model where we will be able to predict whether a recommendation is positive or negative. In this analysis, we will not focus on the Score, but only the positive/negative sentiment of the recommendation. 

1. Data Preprocessing/Clean data:
Remove Special characters
Remove HTML Tags
Removing null coloumn

2. EDA:
bar plot
heatmap

3. 
Applying various Machine Learning models:
LogisticRegression 
RandomForest
KNearestNeighbour
naive bayes

4. sentiment prediction:
Logistic Regression model on Uni-gram/Bi-gram/n-gram bow
Logistic Regression model on TFIDF
Logistic Regression model on TFIDF + n-gram

RandomForest model on Uni-gram/Bi-gram/n-gram bow
RandomForest model on TFIDF
RandomForest model on TFIDF + n-gram

KNeighbors model on Uni-gram/Bi-gram/n-gram bow
KNeighbors model on TFIDF
KNeighbors model on TFIDF + n-gram

MultinomialNB model on Uni-gram/Bi-gram/n-gram bow
