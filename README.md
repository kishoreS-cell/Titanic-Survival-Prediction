# Titanic Survival Prediction — Machine Learning Project

This repository contains an end-to-end Machine Learning pipeline built during my AI & ML internship to predict passenger survival on the Titanic using classification algorithms.

## Dataset Source
The dataset used for this project is the official Kaggle Titanic dataset:
[Kaggle Titanic - Machine Learning from Disaster](https://www.kaggle.com/c/titanic)

## Project Workflow
1. **Data Preprocessing:** Handled missing values (median for Age, mode for Embarked), dropped highly sparse columns (Cabin), and applied label encoding to categorical fields.
2. **Feature Engineering:** Combined `SibSp` and `Parch` variables into a singular `FamilySize` tracking attribute to simplify non-linear model boundaries.
3. **Model Exploration:** Evaluated three distinct classification algorithms: Logistic Regression, Random Forest Classifier, and K-Nearest Neighbors (KNN).

## Evaluation Matrix
| Model | Accuracy | Precision | Recall | F1-Score |
| :--- | :--- | :--- | :--- | :--- |
| **Random Forest** | **0.8268** | **0.7945** | **0.7837** | **0.7891** |
| Logistic Regression | 0.8044 | 0.7826 | 0.7297 | 0.7552 |
| KNN | 0.7206 | 0.7068 | 0.5540 | 0.6212 |

## Conclusion
The Random Forest Classifier emerged as the optimal model, achieving the highest overall accuracy of 82.68% and a well-balanced F1-score of 78.91%. This superior performance is attributed to the ensemble algorithm's capacity to handle complex non-linear feature interactions without overfitting. Ultimately, features such as gender, socio-economic class, and family presence proved to be the most critical determinants of survival probability.
