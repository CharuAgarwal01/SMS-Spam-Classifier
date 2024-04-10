# SMS-Spam-Classifier

## Overview
This repository contains Python code for building a SMS spam classifier using Natural Language Processing (NLP) techniques. The classifier is trained to differentiate between spam and non-spam (ham) messages.

## Steps Followed

1. *Data Loading and Selection*: Loaded the dataset containing SMS messages and selected the required columns - message and label (ham/spam).

2. *Exploratory Data Analysis (EDA)*: Conducted EDA to understand the distribution of spam and ham messages, as well as any patterns or insights that can aid in classification.

3. *Label Encoding*: Converted the label column data to numerical format, where 'ham' is represented as 0 and 'spam' as 1.

4. *Text Preprocessing*: Preprocessed the text data by converting it to lowercase, removing stopwords, and eliminating punctuation from the message column. The preprocessed text was stored in a new column named 'clean_msg'.

5. *Identifying Common Words*: Used the Counter function from the collections library in Python to identify the most common words in both ham and spam messages, aiming to understand the underlying patterns.

6. *Text Vectorization*: Applied CountVectorizer to convert the text data into a document-term matrix using the bag-of-words approach. Further, applied TfidfTransformer to transform the matrix into a TF-IDF representation, giving more weight to rare terms across the corpus.

7. *Model Training*: Employed the Naive Bayes algorithm to train the model on the processed text data.

8. *Evaluation Metrics*: Calculated various evaluation metrics including accuracy score, confusion matrix, and ROC-AUC score to assess the performance of the trained classifier.

9. *Model Comparison*: Explored the performance of other models, such as logistic regression, for comparison purposes.


## Dependencies
- Python 3.x
- pandas
- numpy
- scikit-learn
- matplotlib
- nltk
