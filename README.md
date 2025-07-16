# Customer Churn Prediction in the Telecom Sector

This repository contains the source code, experimental results, and supporting resources for a thesis project titled "Evaluating Machine Learning Techniques for Telecom Customer Churn Prediction." The thesis was submitted in partial fulfillment of the requirements for the degree of Bachelor of Science in Applied Informatics at the University of Macedonia.

## Thesis Overview

The aim of this project is to investigate and evaluate the performance of various machine learning algorithms in predicting customer churn—a key challenge in customer retention efforts in the telecommunications industry. The project focuses on:

- Building predictive models using real-world customer data
- Addressing class imbalance problems through class weighting and oversampling (SMOTE)
- Evaluating the models using metrics such as accuracy, recall, precision, F1-score, and AUC-ROC
- Exploring the effect of feature selection and optimization strategies

## Dataset

The analysis was conducted using the Cell2Cell Churn Dataset, available on Kaggle:  
Kaggle Dataset(https://www.kaggle.com/datasets/jpacse/datasets-for-churn-telecom)

It contains over 50,000 customer records with 58 features including service usage, account information, and demographics.

## Experiments

Five experiments were conducted to systematically analyze different techniques:

1. Baseline Model: Default training on the imbalanced dataset
2. Cost-Sensitive Learning: Use of class weights for minority class emphasis
3. Recall-Oriented Tuning: Hyperparameter optimization using recall as scoring metric
4. SMOTE: Synthetic oversampling of the minority class
5. Top-Feature Modeling: Using only the top 20 features identified by feature importance

All models were evaluated under stratified 5-fold cross-validation.

## Classifiers Used

- Logistic Regression  
- k-Nearest Neighbors  
- Decision Trees  
- Random Forest  
- Naive Bayes  
- Linear Discriminant Analysis  
- AdaBoost  
- Gradient Boosting  
- XGBoost  
- Neural Networks (Keras)

## Results Summary

- XGBoost consistently outperformed other models across all five experiments, achieving the highest F1 scores and strong recall, especially under class weighting and SMOTE.
- Accuracy alone proved misleading due to class imbalance; recall and F1-score were more reliable for evaluating model performance in identifying churners.
- The neural network, when trained with SMOTE, achieved its best performance and lowest loss across all experiments, indicating improved learning stability under balanced conditions.
- Experiments showed that handling class imbalance (via class weighting or SMOTE) is more impactful than tuning scoring metrics alone.

## Project Structure

├── thesis_telecom_churn.ipynb     # Jupyter Notebook with full code and analysis  
├── thesis_churn.pdf               # Complete written thesis  
└── README.md                      # Project description and setup  

## Contact
For questions or collaboration:
- Email: dadakidisgiorgos@gmail.com
- LinkedIn: [https://www.linkedin.com/in/dadakys](https://www.linkedin.com/in/giorgos-dadakidis/)
