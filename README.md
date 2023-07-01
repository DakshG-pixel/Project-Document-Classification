# Project-Text-Classification
I have Implement Naive Bayes on my own from scratch for text classification and Compared the Results with built in Multinomial Naive Bayes in Sklearn.

# Features
* used nltk to import stopwords( to remove the stopwords from our dataset, for better selection of features)
* used nltk.word_tokenize() funtion to convert text in a list of tokens(words)
* selectred the list of important features by selecting their frequency in the dataset
* created a modified 2d matrix of x_dataset with features as columns and row as documents
  * the value at each cell is the count of feature in the document
  * it's easier to calculate the probability of a class from the sum of feature values
* then we use our classifer to fit the given dataset and return a dicitonary that has key's as class's available, which has further keys as feature value and values as the sum of feature value in that particular class,and  the total number of words in each class
* predict, predict_single, probability funciton are used to iteratively calculate each doc's probability of belonging to a prticular class and choosing the class with maximum probability
* implemented laplace's correction
* achieving the accuracy_score of 86% with our classifier

# Dataset Overview
* The Newsgroup dataset is a collection of documents sourced from various newsgroups on Usenet, a distributed discussion system widely used in the early days of the internet. The dataset is commonly employed for text classification tasks and has been widely studied in the field of natural language processing.
* The dataset comprises documents from different newsgroups such as politics, sports, technology, science, and more. Each document represents a post or article contributed by users to the corresponding newsgroup.
* These documents vary in length and can contain a mix of plain text, HTML formatting, and special characters.
* there are 20 catogries each with more than 500 articles in it.

# Split the dataset into training and testing sets:
Used a suitable method to split the dataset into training and testing sets(train-test split from scikit-learn).

# Libraries used in python
sklearn, numpy, matplotlib, nltk, string

# Evaluation
* Calculated evaluation metrics(accuracy, precision, recall, confusion matrix, classification report)to assess the performance of the model.

