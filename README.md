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
2. [Tuned randomforest](data/ISC_RF_tuning.ipynb)
  - Tuned random forest model using Bayesian Optimization
  - Improved recall by 500%, f1 by 100%, and auc by 40%
  - Target-encoded high cardinality categorical variables
3. [Tuned XGBoost](data/ISC_autoopt.ipynb)
  - Set up a XGBoost model pipeline
  - Utilized GPU to improve training time by 600%
  - Models were evaluated in native XGBoost Cross-validation 
## Results

The naive voting classifier model achieved 87.5% accuracy in the public leaderboard. For realistic predictive modeling, the tuned random forest model had an improved recall of 500%, f1 of 100%, and auc of 40% over default model. 


