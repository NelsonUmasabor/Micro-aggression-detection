# Micro Aggression Detection from tweets.


# Table of content

- [Micro Aggression Detection from tweets.](#micro-aggression-detection-from-tweets)
- [Table of content](#table-of-content)
- [Source of Data](#source-of-data)
- [Data Exploration](#data-exploration)
- [Classifier](#classifier)
- [Imbalanced Data](#imbalanced-data)
- [Balanced Data](#balanced-data)
- [Stacking Classifier](#stacking-classifier)

# Source of Data
The dataset is from [Kaggle](https://www.kaggle.com/arkhoshghalb/twitter-sentiment-analysis-hatred-speech) . It is a collection of 31,962 tweets, which have been labelled as either racist/sexist (micro aggression) and non-racist/non-sexist (non-micro aggression) tweets.

# Data Exploration
To better understand the dataset, several plots were used such as:

- A countplot
  
  This is used to see the distribution of various classes of the dataset.

- A wordcloud
  
  This is used to show the most frequent words that show micro aggression and those that do not show micro aggression.

- N-gram Charts

   Bigrams,trigrams and quadgrams of the 20 most frequent words.

- Boxplot

  A boxplot of class distribution by lenght of characters.

# Classifier
-	Linear Support Vector Classifier.
-	Multinomial Naïve Bayes.
-	Random Forest Classifier.
-	Extra Trees Classifier.
-	Light Gradient Boosting (LGBM).
-	Extreme Gradient Boosting (Xgboost).
-	Adaptive Boosting (Adaboost).
-	Logistic Regression.
-	Logistic RegressionCV.
-	Stochastic Gradient Descent (SGD) Classifier.



# Imbalanced Data
- The accuracy scores of the various classifiers are very high with the least being 94%. Apart from the accuracy it is clear that the classifiers were able to classify non-microaggressive tweets perfectly but had trouble classifying microaggressive tweets because the recall for microaggressive tweets is very low. Linear SVC performed the best in classifying racist tweets.

# Balanced Data
- The accuracy scores of the various classifiers are not as high as the accuracy from the imbalanced dataset. The highest accuracy gotten is 88% but the recall is higher than that of the imbalanced dataset. In 6 out of the 10 classifiers used there is better recall for microaggressive tweets.

# Stacking Classifier
- The result of the stacking classifier has shown that combining high performing classifiers may not necessarily outperform individual high performing classifiers. 