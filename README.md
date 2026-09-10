# Diabetes Prediction: From-Scratch Linear & Logistic Regression

Implemented linear regression (Normal Equation) and logistic regression (gradient descent + sigmoid) from scratch using only NumPy/Pandas, with a focus on understanding the underlying math.

**Result:** Logistic regression reached **75.3% accuracy** on the test set.

## Problem
The Pima Indians Diabetes dataset is primarily used for binary classification (diabetic vs not). I first explored single variable linear regression, then multiple linear regression to predict continuous Glucose levels, then built a proper logistic regression classifier for the Outcome variable.

## Approach
- Multiple linear regression via closed-form Normal Equation
- Logistic regression with sigmoid + gradient descent + binary cross-entropy
- Train/test split and scaling.
- Manual confusion matrix and evaluation

## Results
- Logistic regression test accuracy: **75.32%**
- Confusion matrix breakdown: TN 92 | TP 24 | FP 8 | FN 30
- DiabetesPedigreeFunction showed the strongest relationship with Glucose in the linear model

## How to Run
1. Clone the repo
2. `pip install -r requirements.txt`
3. Place `diabetes.csv` in the working directory
4. Run the notebook

## Tech Stack
Python, NumPy, Pandas, Matplotlib (scikit-learn only for train_test_split)

## Limitations & Next Steps
- No hyperparameter tuning or regularization
- Simple threshold of 0.5
- Could add feature engineering
