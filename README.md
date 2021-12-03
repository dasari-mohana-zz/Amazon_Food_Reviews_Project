# Amazon Fine Food Reviews

In this project, I have used different type of Classification models(TSNE, Logistic Regression, SVC, RandomForest, Gradient Boosting Classifier, XGBClassifer, Decision Tree, Naive bayes) are performed on Amazon food reviews dataset with various methods of vectorization to classify postive and negative classes based on customers review text.

## Input Data Source:

https://www.kaggle.com/snap/amazon-fine-food-reviews

## Context:

This dataset consists of reviews of fine foods from amazon. The data span a period of more than 10 years, including all ~500,000 reviews up to October 2012. Reviews include product and user information, ratings, and a plain text review. It also includes reviews from all other Amazon categories.

## Contents:

1.Reviews.csv: Pulled from the corresponding SQLite table named Reviews in database.sqlite

2.database.sqlite: Contains the table 'Reviews'

## Data includes:

Reviews from Oct 1999 - Oct 2012
568,454 reviews
256,059 users
74,258 products
260 users with > 50 reviews

## Attribute Information:

		1.	Id - Unique Id

		2.	ProductId - unique identifier for the product

		3.	UserId - unqiue identifier for the user

		4.	ProfileName

		5.	HelpfulnessNumerator - number of users who found the review helpful

		6.	HelpfulnessDenominator - number of users who indicated whether they found the review helpful or not

		7.	Score - rating between 1 and 5

		8.	Time - timestamp for the review

		9.	Summary - brief summary of the review

		10.	Text - text of the review


## Objective:

Given a review, determine whether the review is positive or negative.

Determine if the review is postive or negative: We could use the Rating/score. A rating of 4 or 5 could be considered as positive review. A review of 1 or 2 could be considered as negative review and rating of 3 is considered as neutral and ignored. This is an approximate and proxy way of determining the polarity (positivity/negativity) of a review.

## MY APPROCH:

1.  Importing the required libraries and reading the dataset.

      a.  Merging of the two datasets

      b.  Understanding the dataset

2.  Exploratory Data Analysis (EDA) –

      a.  Data Visualization

3.  Feature Engineering
 
      a.  Data Cleaning: Deduplication

      b.  Removal of null values

      c.  Text Preprocessing

      d.  Stemming, Stop-word removal and Lemmatization

      e.  Bow of Words

      f.  Word2Vector

      g.  TF-IDF Vectorizer

      h.  Avg W2V, TFIDF-W2V

      i.  T-SNE Analysis

4.  Model Building

      a.  Performing train test split - Time Series Split

      b.  Logistic Regression Model

      c.  KNN Classifier Model

      d.  Naive Bayes Model

      e.  Support Vector Machine Model

      f.  Decision Tree Classifier

      g.  Random Forest Classifier


5.  Hyperparameter Tuning (GridSearchCV and RandomSearch CV)

      a.  For all type of Classifier Models for different type of featurizations(BOW, TF-IDF, AVG W2V)

6.  Model Validation

      a.  Accuracy score

      b.  Confusion matrix

      c.  Area Under Curve (AUC)

      d.  F1-score

7.  Creating the final model and making predictions

8. Conclusion
