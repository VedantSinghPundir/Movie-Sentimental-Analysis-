# Sentiment Analysis App (GUI)

## Overview
This is a Graphical User Interface (GUI) program built using **Tkinter** that allows users to analyze the sentiment of movie reviews. Users can input a review, and the app will classify it as either **Positive** or **Negative** using a pre-trained machine learning model.

---

## Features
- User-friendly GUI for sentiment analysis.
- Error handling to ensure user inputs are valid.
- Utilizes pre-trained Naïve Bayes classification models for sentiment prediction.
- Displays the sentiment analysis result in a pop-up window.

---

## Dependencies
The program uses the following libraries:
- **tkinter**: For creating the GUI.
- **pickle**: For loading the saved vectorizer and model.

---

## Prerequisites
1. **Pre-trained Files**:
   - `count-vectorizer.pkl`: The saved TF-IDF vectorizer.
   - `Movies_Review_Classification.pkl`: The saved classification model.

2. **Python Environment**:
   - Install the required libraries if not already available:
     ```bash
     pip install scikit-learn
     ```

---

## Workflow
1. **GUI Initialization**:
   - Creates a simple interface with:
     - A text entry field for the user to input a movie review.
     - A button to analyze the review.

2. **Review Analysis**:
   - When the user clicks the "Analyze" button:
     - The review is passed to the `test_model()` function.
     - The function uses the pre-trained model and vectorizer to classify the review as **Positive** or **Negative**.

3. **Result Display**:
   - Displays the sentiment result in a pop-up message box.
   - Handles any errors that occur during the process.

---

## Usage
### Running the Program:
1. Ensure the `count-vectorizer.pkl` and `Movies_Review_Classification.pkl` files are in the same directory as the script.
2. Run the program:
   ```bash
   python sentiment_analysis_gui.py
   ```
3. Enter a movie review in the provided input box.
4. Click the "Analyze" button to view the sentiment classification result.

### Example:
- Input: *"This is the best movie I have ever watched."*
- Output: *"Positive review"*

---

## Code Highlights
### Key Functions:
1. **`analyze_review()`**:
   - Handles the input from the user.
   - Calls `test_model()` to analyze the sentiment.
   - Displays the result or error message in a pop-up window.

2. **`test_model(sentence)`**:
   - Transforms the input text using the saved TF-IDF vectorizer.
   - Predicts the sentiment using the saved classification model.
   - Returns "Positive review" or "Negative review."

### GUI Components:
- **Label**: Displays instructions for the user.
- **Entry**: Accepts user input (movie review).
- **Button**: Triggers the sentiment analysis process.

---

## Future Improvements
- Add support for batch review analysis.
- Enhance the GUI design with more styling options.
- Include additional metrics or visualizations for analysis results.
- Deploy the app as a standalone executable using tools like **PyInstaller**.

---

## License
This project is licensed under the MIT License.
