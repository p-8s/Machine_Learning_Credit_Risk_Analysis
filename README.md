

## Task Description

This project aims to apply and compare different machine learning models in the field of Probability of Default (PD) analysis for consumer lending. Starting from the baseline logistic regression, we compared the AUC-ROC curve for regression models, Support Vector Machine (SVM) and tree-based methods.

### Background

Understanding risk of default is a crucial part of credit scoring before onboarding a customer for credit card products and services. If a borrower presents an acceptable level of default risk, the bank can recommend the approval of their credit application and grant a suitable credit limit. Using logistic regression for credit analysis has been an established practice in banking. While it clearly enjoys the inherent benefit of high interpretability, it in general suffers from a lower accuracy than more advanced machine learning methods.

Interested in examining the performance of different classification models and their applicability in the banking industry, we modelled default risk using regression, SVM and decision trees on a sample dataset available on [Kaggle](https://www.kaggle.com/rikdifos/credit-card-approval-prediction). Subsequently, we compared their respective computational speed, interpretability, predictive accuracy, robustness to outliers and ability to handle irrelevant features.


## Our Approach

We developed three main groups of models: regression, SVM and decision tree ensembles.

Regression

- Baseline logistic model with 2 predictors: developed using gradient descent
- Logistic regression after best subset variable selection
- Logistic regression after stepwise variable selection
- LASSO regression

SVM

- SVM using radial kernel

Tree-based methods

- Single decision tree
- Bagging ensemble with decision trees
- Random forest ensemble with decision trees

Finally, we concluded with a model comparison. LASSO regression was our recommended model. Being a regularised method, it outperformed logistic regression developed after stepwise/best subset variable selection in terms of accuracy, and kept the benefits of high interpretability. Random forest was the best performing model in terms of AUC-ROC curve. However, its likelihood of adoption in Banking is low due to the highly regulated nature of the industry, and the "black-box" nature of the algorithm. 

