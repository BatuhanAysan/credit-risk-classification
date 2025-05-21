# Credit Risk Classification

## Overview

This analysis uses logistic regression to predict the credit risk of loan applicants using historical data from a peer-to-peer lending company. The goal is to classify loans into two categories:

- `0`: Healthy loan (low risk of default)
- `1`: High-risk loan (high risk of default)

By training a machine learning model, the company can make more informed lending decisions and minimize financial losses.

---

## Results

- **Accuracy Score**: 0.99
- **Precision Score**:
  - Healthy Loans (0): 1.00
  - High-Risk Loans (1): 0.85
- **Recall Score**:
  - Healthy Loans (0): 0.99
  - High-Risk Loans (1): 0.91

---

## How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?

The logistic regression model performs exceptionally well in predicting both classes, with an overall **accuracy of 99%**.

- For **healthy loans (label 0)**:
  - **Precision:** 1.00  
  - **Recall:** 0.99  
  - This indicates the model can almost perfectly identify low-risk loans.

- For **high-risk loans (label 1)**:
  - **Precision:** 0.85  
  - **Recall:** 0.91  
  - This shows the model correctly identifies 91% of high-risk loans, though it sometimes misclassifies them as healthy.

**Summary:**  
The model is very reliable for identifying both healthy and high-risk loans. While performance is slightly lower for high-risk predictions, this is a common tradeoff when dealing with imbalanced datasets. Overall, the model provides trustworthy results for initial credit risk assessment.

---

## Recommendation

Based on its high accuracy and strong performance across both loan categories, the logistic regression model is a solid starting point for credit risk classification. It can be confidently used in production with periodic performance reviews. Future work could explore alternative models (e.g., Random Forest, XGBoost) and further address class imbalance to improve high-risk prediction even more.
