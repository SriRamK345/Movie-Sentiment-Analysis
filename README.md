# Movie Review Sentiment Analysis

## Overview

This project performs sentiment analysis on movie reviews to classify them as either positive or negative. It uses a dataset of movie reviews from NLTK and employs a machine learning pipeline with TF-IDF vectorization and a Multinomial Naive Bayes classifier.

## Dataset

The dataset used in this project is the "movie_review" dataset from NLTK, downloaded using the Kaggle API. It contains labeled movie reviews, where each review is tagged as either "pos" (positive) or "neg" (negative).

## Preprocessing

The following preprocessing steps are applied to the movie review text:

1. **Contraction Expansion:** (Currently commented out in the code) Contractions like "can't" are expanded to their full forms (e.g., "cannot").
2. **Number Removal:** Numbers are removed from the text.
3. **Punctuation Removal:** Punctuation marks are removed.
4. **Lowercasing:** Text is converted to lowercase.
5. **Stop Word Removal:** Common English stop words (like "the", "a", "is") are removed.
6. **Lemmatization:** Words are reduced to their base forms using WordNetLemmatizer.

## Model Training

A machine learning pipeline is used for sentiment analysis:

1. **TF-IDF Vectorization:** Text data is transformed into numerical features using TF-IDF (Term Frequency-Inverse Document Frequency).
2. **Multinomial Naive Bayes Classifier:** A Multinomial Naive Bayes classifier is trained on the vectorized data to predict sentiment.

## Evaluation

The model is evaluated using metrics like accuracy and a classification report. Word clouds are generated to visualize the most frequent words in positive and negative reviews.

## Usage

To use the sentiment analysis model, provide a movie review as input. The model will predict whether the review is positive or negative.
