# WasteLess Models

This repository contains various machine learning models trained on the `mess_feedback_forms.csv` dataset to predict sentiment and waste probability based on student feedback.

## Dataset
The models utilize a dataset of mess feedback forms containing both textual feedback and numerical ratings regarding hygiene, portion sizes, main dishes, and overall experience.

## Models Implemented

| Model Name | Description | Accuracy (%) |
| :--- | :--- | :--- |
| **Random Forest** | Predicts High Waste or Low Waste using multiple decision trees. | 98.75% |
| **TF-IDF** | Converts textual feedback into numerical importance scores for NLP processing. | 88.75% |
| **Bayesian Model** | Predicts sentiment and waste probability using probabilistic reasoning | 88.75% |
| **RNN** | Understands sentence context and predicts sentiment using deep learning | 88.75% |
| **K-MEANS CLUSTERING** | Groups students into similar behavioral clusters automatically | 86.42% |

## Best Performing Model
The **Random Forest** model achieved the highest accuracy of **98.75%**. It efficiently predicts High Waste or Low Waste by assessing factors such as hygiene ratings, sentiment scores, and menu variables.

## Features Extracted
The following features were processed for the models (especially Random Forest):
- Textual Feedback (cleaned and vectorized using TF-IDF)
- Feedback Length
- Mess Hygiene Ratings
- Overall Satisfaction (Ratings)
- Encoded Menu Items and Portion Sizes
- Negative Word Counts & Sentiment Scores

## Usage
1. Ensure you have the required Python libraries installed:
   * pandas
   * scikit-learn
   * matplotlib
   * numpy
2. Load the dataset mess_feedback_forms.csv into the same directory as the notebook.
3. Run the notebook cells sequentially to train and evaluate each model.
