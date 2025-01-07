# Sentiment Classification Using Logistic Regression

## Overview

This project implements sentiment classification for hotel reviews using:

- **Logistic Regression** (with PyTorch) for binary classification (positive vs. negative sentiment).
- **Naive Bayes Classifier** and **Random Chance Classifier** as baseline models.

The input is a text review, and the output is a binary label: `1` (positive) or `0` (negative).

---

## Workflow

### Dataset Exploration:
- Reviews are loaded from positive and negative files.
- Distribution of labels is analyzed to ensure balanced splits.

### Feature Engineering:
- Extracted features like word counts, review length, exclamation marks, and positive/negative word counts.
- Normalized features for consistency.

### Baseline Models:
- **Random Chance Classifier** predicts labels based on distribution.
- **Naive Bayes Classifier** uses token frequencies for predictions.

### Logistic Regression:
- Implemented using PyTorch with hand-engineered features.
- Optimized with **Stochastic Gradient Descent (SGD)** and evaluated using **Accuracy**, **Precision**, **Recall**, and **F1-score**.

---

## Key Results

### Baseline Models:
- **Random Chance F1-score**: ~0.33
- **Naive Bayes F1-score**: ~0.72

### Logistic Regression:
- **Development Set F1-score**: ~0.91
- **Test Set F1-score**: ~0.90

---

## Sample Reviews

- **Positive Example**: "The hotel was amazing, clean, and had great service!"
- **Negative Example**: "The room was dirty, and the staff was rude."

---

## Technologies Used

- **Python**: Core programming language.
- **PyTorch**: Logistic Regression implementation.
- **NumPy**: Data manipulation.
- **Sklearn**: Dataset splitting and evaluation metrics.

