# Predicting Insurance Cross Sell

## Project description

Welcome to the Insurance Cross Sell Prediction project! This repository contains the code, data, and documentation for a machine learning analysis aimed at predicting whether a customer will buy services from their existing insurance provider (i.e., cross sell). Accurately predicting cross sell is crucial for insurance business to improves sales and revenue.

## Objective

The main objective of this project is to develop a predictive model that can classify customers into two categories: those who will likely buy additional services and those who won't. By identifying these customers, businesses can implement targeted interventions to sell their services.

![Bank Churn](assets/sales.jpg)

## Dataset

The dataset used in this project belongs to the [Kaggle Playground Series](https://www.kaggle.com/competitions/playground-series-s4e7/overview). The data includes various features that might influence a customer's decision to buy more services, such as:

- Customer demographics (Age, gender, etc.)
- Customer information (Previously insured, vehicle age,  etc.)

## Methods

We evaluated the performance of the following models in predicting insurance cross sell:

1.[Voting classifier](data/ISC_naive_clf.ipynb)
  - 8 Default classifiers were compared on performance
  - Top 3 models were used in a soft-probability vote classifier
2. [Tuned XGBoost](data/ISC_autoopt.ipynb)
  - Set up a XGBoost model pipeline
  - Used Bayesian hyperoptimization to tune model
  - Models were evaluated in native XGBoost Cross-validation
3. [Tuned randomforest](data/ISC_RF_tuning.ipynb)
  - Work in progress
  
## Results

1. The naive voting classifier model achieved 87.5% accuracy in the public leaderboard.


