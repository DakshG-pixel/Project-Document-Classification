# Project-Text-Classification
I have Implement Naive Bayes on my own from scratch for text classification and Compared the Results with built in Multinomial Naive Bayes in Sklearn.

# Features
* Stopword Removal: Stopwords are imported using the NLTK library to remove them from the dataset, improving feature selection.
* Tokenization: The text is converted into a list of tokens (words) using nltk.word_tokenize() function.
* Feature Selection: Important features are selected based on their frequency in the dataset.
* Modified 2D Matrix: A modified matrix is created with features as columns and documents as rows, storing the count of each feature in each document.
* Probability Calculation: Probability of a document belonging to a class is calculated by summing the feature values.
* Naive Bayes Classifier: The classifier fits the dataset and returns a dictionary representing classes, features, and their respective counts.
* Prediction: Functions predict, predict_single, and probability are used to calculate the probability of each document belonging to a class and predict the class with maximum probability.
* Laplace's Correction: Laplace's correction is implemented to handle unseen features and zero probabilities.

# Dataset Overview
The Newsgroup dataset consists of documents from different newsgroups on Usenet, commonly used for text classification. Each document represents a post or article from a specific newsgroup. The dataset is sourced from various categories like politics, sports, technology, and science. Documents may contain plain text, HTML formatting, and special characters.
 * there are 20 catogries each with more than 500 articles in it.

# Split the dataset into training and testing sets:
Used a train-test split method from scikit-learn to split the dataset into training and testing sets.

# Libraries Used
The project utilizes the following Python libraries:
* sklearn: Used for implementing the train-test split and evaluating the model's performance.
* numpy: Used for numerical computations and array operations.
* matplotlib: Used for visualizations and plotting.
* nltk: Used for natural language processing tasks, such as tokenization and stopwords removal.
* string: Used for string manipulation and formatting.

# Evaluation
I calculated various evaluation metrics, including accuracy, precision, recall, confusion matrix, and classification report, to assess the performance of the model. These metrics provide insights into the model's effectiveness in correctly classifying the documents.

Feel free to explore the code and modify it to suit your specific requirements. The project offers a practical implementation of text classification using Naive Bayes and provides a starting point for further experimentation and improvement.

Please refer to the project's code and documentation for detailed usage instructions and examples.

