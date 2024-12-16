# Sentiment Analysis on IMDB Movie Reviews

## Overview
This program performs sentiment analysis on the IMDB movie review dataset. It classifies reviews as either **positive** or **negative** using natural language processing (NLP) techniques and machine learning algorithms. The program uses the Naïve Bayes classification family (GaussianNB, MultinomialNB, BernoulliNB) to evaluate the best-performing model for this task.

---

## Features
- Data Preprocessing: Cleans and preprocesses the text data, including stemming and removing stopwords.
- Exploratory Data Analysis (EDA): Displays the distribution of sentiments in the dataset using pie charts.
- Feature Extraction: Converts text into numerical features using the **TF-IDF Vectorizer**.
- Machine Learning Models: Trains and evaluates multiple Naïve Bayes classifiers.
- Performance Metrics: Calculates accuracy, confusion matrix, and weighted precision.
- Model Serialization: Saves the best-performing model and vectorizer for future use.
- Real-time Testing: Includes a function to classify new reviews as positive or negative.

---

## Dependencies
The program uses the following libraries:
- **pandas**: For data handling and analysis.
- **numpy**: For numerical computations.
- **nltk**: For natural language processing tasks.
- **scikit-learn**: For machine learning models and evaluation metrics.
- **matplotlib**: For visualization.
- **pickle**: For saving and loading models and vectorizers.

---

## Dataset
The IMDB Dataset (`IMDB Dataset.csv`) is used, which contains:
- **review**: The text of the movie review.
- **sentiment**: The sentiment of the review (Positive or Negative).

---

## Workflow
1. **Load Dataset**:
   - Reads the dataset and checks for missing values.
   - Displays the overall sentiment distribution.

2. **Data Preprocessing**:
   - Converts text to lowercase and removes non-alphabetic characters.
   - Tokenizes text and removes stopwords using NLTK.
   - Stems words to their root forms using Porter Stemmer.

3. **Feature Extraction**:
   - Uses **TF-IDF Vectorizer** to transform text data into numerical features.

4. **Model Training**:
   - Splits the dataset into training and testing sets (80:20).
   - Trains three Naïve Bayes models: GaussianNB, MultinomialNB, BernoulliNB.
   - Evaluates each model using accuracy, confusion matrix, and weighted precision.

5. **Model Serialization**:
   - Saves the vectorizer and the best-performing model (BernoulliNB) using `pickle`.

6. **Testing New Reviews**:
   - Implements a function `test_model(sentence)` to classify new reviews as **Positive** or **Negative**.

---

## Visualizations
A pie chart displays the distribution of positive and negative reviews to provide an overview of the dataset.

---

## Results
- **MultinomialNB** achieved the highest accuracy and precision among the models tested.
- The program classifies new movie reviews effectively.

---

## Usage
### Running the Program:
1. Ensure all dependencies are installed.
2. Place the `IMDB Dataset.csv` file in the same directory.
3. Run the program to:
   - Preprocess the data.
   - Train the models.
   - Save the best model and vectorizer.

### Testing New Reviews:
Use the `test_model(sentence)` function:
```python
sen = 'This is a wonderful movie I have seen'
res = test_model(sen)
print(res)  # Output: Positive review
```

### Serialized Files:
- **count-vectorizer.pkl**: Saved TF-IDF Vectorizer.
- **Movies_Review_Classification.pkl**: Saved BernoulliNB model.

---

## Future Improvements
- Extend the model to handle neutral sentiments.
- Explore advanced NLP models such as Transformers (e.g., BERT).
- Visualize word clouds for positive and negative reviews.
- Deploy the model as a web application for interactive testing.

---

## License
This project is licensed under the MIT License.

