# Parkinson’s Disease Voice Classification

## Project Overview
This project applies machine learning techniques to classify Parkinson’s Disease (PD) using voice signal features.  
Voice impairment is one of the earliest symptoms of Parkinson’s Disease, making voice-based analysis a promising approach for early detection.

The goal of this project is to compare multiple classification models and evaluate their performance in identifying Parkinson’s patients from vocal data.

## Dataset

Parkinson’s Speech Dataset  
Source: UCI Machine Learning Repository

The dataset contains voice recordings of individuals with and without Parkinson’s Disease. 
Each sample includes acoustic features extracted from sustained vowel phonations.

---

## Methods

The following machine learning models were implemented and evaluated:

- Naïve Bayes (GaussianNB)
- K-Nearest Neighbors (KNN)
- Artificial Neural Network (MLPClassifier)

Key steps in the workflow included:

- Exploratory Data Analysis (EDA)
- Feature selection using ANOVA F-test
- Correlation filtering to remove redundant features
- Data standardization using StandardScaler
- Model training and evaluation
- Performance comparison across models

---

## Key Results

| Model | Accuracy | Recall (PD) |
|------|------|------|
| Naïve Bayes | 81.1% | 0.92 |
| KNN (k=7) | 83.0% | 0.95 |
| MLP (Neural Network) | **83.69%** | 0.94 |

The MLP model achieved the best overall performance with the most balanced results across metrics.

---

## Key Insights

- All models showed strong ability to detect Parkinson’s cases.
- Class imbalance made it more difficult to correctly identify healthy individuals.
- The neural network model produced the most consistent performance across validation folds.
- Minimizing false negatives is particularly important in medical screening contexts.

---

## Tools & Technologies

Python  
Pandas  
Scikit-learn  
Matplotlib  
Jupyter Notebook  

Machine Learning Models:
- KNN
- Naïve Bayes
- Artificial Neural Networks (MLP)
