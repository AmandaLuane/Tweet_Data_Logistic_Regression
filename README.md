# Sentiment Analysis Pipeline

## Overview

This repository contains code for a sentiment analysis pipeline designed to analyze sentiment in Twitter data. The pipeline preprocesses the data, extracts features using TF-IDF, and trains logistic regression models to classify tweets as expressing positive or negative sentiment.

## Features

- Data preprocessing: Cleaning and standardizing tweet text by removing mentions, URLs, punctuation, numbers, and non-ASCII characters, converting text to lowercase, stripping whitespace, and lemmatizing words.
- Feature extraction: Using TF-IDF Vectorizer to convert preprocessed text data into numerical features.
- Model training: Training logistic regression models on the TF-IDF features to classify tweets into positive or negative sentiment categories.
- Model evaluation: Assessing the performance of the trained models using accuracy metrics on both training and testing datasets.
- Parameter tuning: Exploring the impact of different settings for the `max_features` parameter in the TF-IDF Vectorizer.

## Usage

1. Clone the repository to your local machine:

    ```bash
    git clone https://github.com/your_username/sentiment-analysis-pipeline.git
    ```

2. Install the required dependencies using `pip`:

    ```bash
    pip install -r requirements.txt
    ```

3. Run the Jupyter notebook or Python script to execute the sentiment analysis pipeline.

## Dataset

The pipeline uses labeled tweet data obtained from two different sources:

- Keyword-based tweets: Contains tweets labeled as expressing positive ("POLIT") or negative ("NOT") sentiment based on specific keywords.
- General tweets: Contains tweets labeled as expressing positive ("POLIT") or negative ("NOT") sentiment based on general content.

## Results

The pipeline evaluates the performance of the sentiment analysis models using accuracy metrics on the training and testing datasets. Additionally, it explores the impact of varying the `max_features` parameter in the TF-IDF Vectorizer on model performance.
