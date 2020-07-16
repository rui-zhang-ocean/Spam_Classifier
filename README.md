# Spam Detection on SMS messages 

![spam-can](https://github.com/rui-zhang-ocean/Spam_Classifier/blob/master/figs/spam-can.png)

### Summary
This project aims to test a range of NLP vectorizers and classifiers on spam detection using data created by [Tiago A. Almeida and José María Gómez Hidalgo](http://www.dt.fee.unicamp.br/~tiago/smsspamcollection/). 

2 vectorizers:
 - Bag of Words
 - TF-IDF 

5 classifiers:
 - Logistic Regression
 - SVC
 - K-Neighbour
 - NaiveBayes
 - RandomForest

The classifier parameters are already optimized, which are based on notebook:
[Spam detection Classifiers hyperparameter tuning](https://www.kaggle.com/muzzzdy/d/uciml/sms-spam-collection-dataset/spam-detection-classifiers-hyperparameter-tuning/)

### Steps
 - Import data and remove unnecessary columns.
 - Exploratory data analysis including ham (legitimate) and spam messages count and length.
 - Pre-process data including removal of punctuations and stopwords
 - Set-up work flow
     - feature extraction using vectorizer
     - split data into train and test set
     - train classifier using training dataset
     - predict labels for test set using trained classifier
     - calculate accuracy score 
 - Loop through the work flow using 2 vectorizers and 5 classifiers
 - Visualize and compare the results.
 
### Results
![accuracy_score_barplot](https://github.com/rui-zhang-ocean/Spam_Classifier/blob/master/figs/accuracy_score.png)

**Naive Bayes** classifier with **TF-IDF** vectorizer outperforms other approaches with an accuracy score of **0.98**
