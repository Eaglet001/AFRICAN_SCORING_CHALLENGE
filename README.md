# Bluechip Data & AI 2024 Summit Hackathon
machine learning model to predict the likelihood of loan defaults for both existing customers and new applicants

## Table of Contents
- [Introduction](#introduction)
- [Feature_Engineering](#feature_engineering)
- [Model](#model)
- [Technologies](#technologies)

## Introduction
The primary objective of this hackathon is to develop accurate and robust machine learning models that can predict the creditworthiness of a borrower. The goal is to identify individuals who are most likely to repay loans while reducing the risk for financial institutions. Participants will be judged on their model’s ability to make accurate predictions, their approach to feature engineering, and how well they handle the trade-off between precision and recall.

## Feature_Engineering
The dataset was checked for missing values whcih it has none,while EDA was performed to check important information about the data and it variables. The following Feature Engineering was done to the data using the following : 
- ### label Encoder
from sklearn.preprocessing import LabelEncoder
- label_encoder = LabelEncoder()
- train_b.loc[:,'Dependents_N'] = label_encoder.fit_transform(train_b['Dependents'].astype(str))
- test_b.loc[:,'Dependents_N'] = label_encoder.fit_transform(test_b['Dependents'].astype(str))


## Model
The model for this use case was built using Random forest and evaluated on Accuracy
The model gave an accuracy score on the private 0.83926 and 0.83436 public leaderboard 

The model performance on the purespectively , placing me 47th in the competition out of 230 participants 


## Technologies
- jupyter notebook
- python
- Pandas
- Skick_learn
### link to the hackathon
https://www.kaggle.com/competitions/bluechip-summit-credit-worthiness-prediction/leaderboard

