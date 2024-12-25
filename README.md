This project demonstrates a machine learning approach to predict the gender of a person based on their name using various text vectorization techniques and classification algorithms.
Project Overview

Names often carry subtle patterns that can be associated with gender. This project explores these patterns by leveraging natural language processing (NLP) techniques and machine learning models. The workflow includes preprocessing names, extracting meaningful features, and training a classifier to predict gender labels.
Features

Preprocessing of name data into vectorized formats.
Use of multiple feature extraction techniques:
CountVectorizer: Character n-grams to capture patterns in names.
TF-IDF Vectorizer: Weighted representation of character n-grams to emphasize unique patterns.
DictVectorizer: Encoding categorical data for better feature handling.
Training using Multinomial Naive Bayes classifier.
Key Components

1. Models and Vectorizers Used
MultinomialNB: A probabilistic model for classification that works well with categorical and text data.
CountVectorizer: Converts text into a sparse matrix of token counts.
TfidfVectorizer: Enhances text representation by scaling token counts with inverse document frequency (IDF).

2. Workflow
Load the dataset of names and corresponding gender labels.
Preprocess and vectorize the names using the following methods:
CountVectorizer: Character-level n-grams (e.g., bi-grams, tri-grams).
TfidfVectorizer: Adds weight to rare but meaningful patterns in names.
Train a Multinomial Naive Bayes (MultinomialNB) classifier on the vectorized data.
Evaluate the model using accuracy, precision, recall, and F1-score metrics.
Test the model with unseen names to predict gender.
