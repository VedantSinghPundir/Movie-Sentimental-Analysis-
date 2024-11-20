# Movie Sentiment Analysis with GUI Application

This project performs sentiment analysis on IMDB movie reviews using Natural Language Processing (NLP) techniques and machine learning. It also includes a user-friendly **GUI application** built with Tkinter to analyze movie reviews interactively.

---

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
  - [Using the Script](#using-the-script)
  - [Using the GUI Application](#using-the-gui-application)
- [Results](#results)

---

## Overview

This project uses machine learning models and NLP techniques to classify movie reviews as **Positive** or **Negative** based on their sentiment. The project includes:
1. A Python script for training and testing the models.
2. A GUI application for interactive sentiment analysis.

---

## Features
- Cleans and preprocesses text data using:
  - Stopword removal
  - Stemming with the `PorterStemmer`
- Visualizes dataset distributions with Matplotlib.
- Trains and evaluates multiple Naive Bayes classifiers:
  - MultinomialNB
  - GaussianNB
  - BernoulliNB
- GUI application built with Tkinter to allow real-time analysis of reviews.
- Models and vectorizers are serialized with Pickle for reusability.

---

## Technologies Used

- **Programming Language:** Python
- **Libraries:** 
  - Pandas
  - NumPy
  - NLTK
  - Scikit-learn
  - Matplotlib
  - Pickle
  - Tkinter

---

## Dataset

The project uses the [IMDB Dataset](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews), which contains 50,000 labeled movie reviews:
- **Columns:**
  - `review`: The text of the movie review.
  - `sentiment`: The sentiment of the review (Positive/Negative).

### Dataset Distribution
- **Positive Reviews:** 25,000
- **Negative Reviews:** 25,000

---

## Installation

Follow these steps to set up the project locally:

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/movie-sentiment-analysis.git
    ```
2. Navigate to the project directory:
    ```bash
    cd movie-sentiment-analysis
    ```
3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```
4. Download the IMDB dataset and save it in the project directory as `IMDB Dataset.csv`.

---

## Usage
## Using the Script
1. Run the script to preprocess the data and train models:
    ```bash
    python movie_sentiment_analysis.py
    ```
2. Use the saved model to classify new reviews:
    ```python
    from test_model import test_model

    # Example usage
    print(test_model("This is the best movie I have ever seen!"))  # Output: Positive review
    print(test_model("The movie was terrible and boring."))       # Output: Negative review
    ```
## Using the GUI Application
1. Launch the GUI application :
    ```python
    sentiment_analysis_app.py
    ```
2. Enter a movie review in the input box and click Analyze.

3. View the result (Positive/Negative sentiment) in a pop-up window.


---

## Results

The trained models achieved the following accuracy on the test set:
- **MultinomialNB:** 85.18%
- **GaussianNB:** 78.55%
- **BernoulliNB (Best Model):** 85.25%

### Confusion Matrix (Best Model: BernoulliNB)
### Weighted Precision:
- **BernoulliNB:** 85.27%

---
