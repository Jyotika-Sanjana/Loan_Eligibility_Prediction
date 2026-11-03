# 🏦 Loan Eligibility Prediction using Machine Learning

A machine learning project that predicts whether a loan applicant is likely to be approved, with a Streamlit web app where users can sign up, log in and check their eligibility.

## Why this project
Banks review a large number of loan applications every day, and manual checks are slow and error-prone. This project automates the first screening step by learning from past applicant data to predict loan status (approved / not approved).

## Features used
Gender · Marital Status · Dependents · Education · Employment Status · Applicant Income · Co-applicant Income · Loan Amount · Loan Amount Term · Credit Score/History · Property Area

## Project structure
| File | Purpose |
|---|---|
| `Loan Eligibility Prediction.ipynb` | Data exploration, preprocessing, model training and evaluation |
| `DataLoanGithub.csv` | Dataset of past loan applications |
| `webpage.py` | Streamlit app with login/signup (SQLite) and the loan prediction form |

## Approach
1. **Data cleaning:** handled missing values and encoded categorical features
2. **Exploration:** studied how credit history, income and property area relate to approval
3. **Modelling:** trained and compared Logistic Regression, KNN, SVC, Random Forest and Decision Tree classifiers
4. **Deployment:** wrapped the model in a Streamlit app that returns an instant eligibility result

## Model comparison
| Model | Test Accuracy |
|---|---|
| **Logistic Regression** | **83.77%** |
| K-Nearest Neighbors | 83.12% |
| Support Vector Classifier | 81.17% |
| Random Forest | 79.87% |
| Decision Tree | 72.73% |

Logistic Regression scored highest, but KNN is within a single percentage point, so the two are effectively comparable on this test set. Logistic Regression was chosen as the final model for its simplicity and interpretability. The Decision Tree performed noticeably worse than the other models.

## Tech stack
Python · Pandas · NumPy · Scikit-learn · Streamlit · SQLite · Jupyter Notebook
