# Amazon fine food review Sentiment Analysis
 
This dataset consists of reviews of fine foods from amazon. The data span a period of more than 10 years, including all ~500,000 reviews up to October 2012. Reviews include product and user information, ratings, and a plain text review. It also includes reviews from all other Amazon categories.

## Data includes:

Reviews from Oct 1999 - Oct 2012<br/>
568,454 reviews<br/>
256,059 users<br/>
74,258 products<br/>
260 users with > 50 reviews<br/>

## attributes describe: 
<br/>
1.Id<br/>
2.ProductId - unique identifier for the product<br/>
3.UserId - unqiue identifier for the user
4.ProfileName<br/>
5.HelpfulnessNumerator - number of users who found the review helpful<br/>
6.HelpfulnessDenominator - number of users who indicated whether they found the review helpful or not<br/>
7.Score - rating between 1 and 5<br/>
8.Time - timestamp for the review<br/>
9.Summary - brief summary of the review<br/>
10.Text - text of the review<br/>

https://www.kaggle.com/snap/amazon-fine-food-reviews

The purpose of this analysis is to make up a prediction model where we will be able to predict whether a recommendation is positive or negative. In this analysis, we will not focus on the Score, but only the positive/negative sentiment of the recommendation. 


## Data Preprocessing/Clean data:<br/>
Remove Special characters<br/>
Remove HTML Tags<br/>
Removing null coloumn<br/>

## EDA:<br/>
bar plot<br/>
heatmap<br/>

## Applying various Machine Learning models:<br/>
LogisticRegression <br/>
RandomForest<br/>
KNearestNeighbour<br/>
naive bayes<br/>

## Sentiment prediction:<br/>
Logistic Regression L1 model on Uni-gram/Bi-gram/n-gram bow<br/>
Logistic Regression L1 model on TFIDF<br/>
Logistic Regression L1 model on TFIDF + n-gram<br/>

Logistic Regression L2 model on Uni-gram/Bi-gram/n-gram bow<br/>
Logistic Regression L2 model on TFIDF<br/>
Logistic Regression L2 model on TFIDF + n-gram<br/>

RandomForest model on Uni-gram/Bi-gram/n-gram bow<br/>
RandomForest model on TFIDF<br/>
RandomForest model on TFIDF + n-gram<br/>

KNeighbors model on Uni-gram/Bi-gram/n-gram bow<br/>
KNeighbors model on TFIDF<br/>
KNeighbors model on TFIDF + n-gram<br/>

MultinomialNB model on Uni-gram/Bi-gram/n-gram bow<br/>

## Conclusion:<br/>
Achieved the highest accuracy score of 94.5%, F1 score of 94% and AUC score of 96.5% with Logistic Regression L2 on Bi-gram model based on positive/negative reviews prediction

## Updated Version:<br/>
In the updated version, I applied gridsearch to tune the parameter
The best model in this case is Logistic Regression L2 on Bi-gram + TFIDF model, the accuracy score is 95.4%, AUC score is 98%, f1 score is 97.3%
