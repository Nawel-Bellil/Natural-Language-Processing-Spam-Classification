

# Spam Classification using Logistic Regression

## Overview

This project focuses on classifying emails as spam or legitimate (ham) using logistic regression. It involves several steps, including data preprocessing, feature extraction, model training, and evaluation.

## Data Preprocessing

- The emails are preprocessed to remove stopwords, punctuation, and non-sense words using NLTK.
- Tokenization and lemmatization are performed to normalize the text data.
- The emails are converted into a features matrix using a count vectorizer.

## Feature Extraction

- The count vectorizer converts the text data into numerical features representing the frequency of each token.
- The feature matrix is normalized using Min-Max scaling to ensure consistency across features.

## Model Training

- Logistic regression is applied to the training data to build a classification model.
- The trained model is evaluated using the test data, and a classification report is generated to assess its performance.

## Evaluation

The model's performance on the test data is as follows:

|     Class     | Precision | Recall | F1-Score | Support |
|---------------|-----------|--------|----------|---------|
|       0       |    0.85   |  0.99  |   0.91   |   558   |
|       1       |    0.91   |  0.40  |   0.55   |   168   |
|    Accuracy   |           |        |   0.85   |   726   |
|   Macro Avg   |    0.88   |  0.69  |   0.73   |   726   |
| Weighted Avg |    0.86   |  0.85  |   0.83   |   726   |

The classification report provides insights into the model's performance, including precision, recall, F1-score, and support for both spam and legitimate classes.

## Conclusion

This project demonstrates an end-to-end process for spam classification using logistic regression. By preprocessing the data, extracting meaningful features, and training a classification model, it offers a systematic approach to identifying spam emails.

