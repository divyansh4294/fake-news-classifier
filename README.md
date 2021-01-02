# Fake News Classifier

Fake News Classifier in Python
In this project, we have used various natural language processing techniques and machine learning algorithms to classify fake news articles using sci-kit libraries from python.

## Dataset Used

train.csv: A full training dataset with the following attributes:

* id: unique id for a news article
* title: the title of a news article
* author: author of the news article
* text: the text of the article; could be incomplete
* label: a label that marks the article as potentially unreliable
  * 1: unreliable
  * 0: reliable

## File Descriptions

### CountVectorizer_TFIDFVectorizer.ipynb

This file contains all the pre processing functions needed to process all input documents and texts.
* First we read the train file then performed some pre processing like tokenizing, stemming etc.
* Remove all nan values
* Apply feature extraction techniques:
	* CountVectorizer
	* TFIDFVectorizer


Here we have build all the classifiers for predicting the fake news detection.
The extracted features are fed into different classifiers.
We have used Multinomial Naive-bayes, passive aggressive classifier algorithm from sklearn.
Each of the extracted features were used in all of the classifiers.
Once fitting the model, we compared the accuracy and checked the confusion matrix.
After fitting all the classifiers, best performing models were selected as candidate models for fake news classification. 
Finally selected model was used for fake news detection with the probability of truth.

### fake_news_classifier_using_lstm.ipynb

Here we have build all the classifiers for predicting the fake news detection.
The extracted features are fed into different classifiers.
We have used LSTM model.
Each of the extracted features were used in all of the classifiers.
Once fitting the model, we compared the accuracy and checked the confusion matrix.



