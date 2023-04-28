# Credit Risk Classification - Module 20
![credit](https://finscience.com/wp-content/uploads/il-ruolo-degli-alternative-data-nel-credit-risk-management-finscience-datrix.jpg)

## Intro
In this Challenge, we were to utilize various techniques to train and evaluate a model based on loan risk. We used a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

## Analysis

## Logistics Regression Original Data vs Resampled Training Data

### Logistics Regression Original Data Classification Report

- Label 0
    - Precision: 1.00 
    - Recall:  0.99 
    - F1-score: 1.00 

- Label 1
    - Precision: 0.85 
    - Recall:  0.91
    - F1-score: 0.88

### Logistics Regression Resampled Training Data Classification Report

- Label 0
    - Precision: 1.00 
    - Recall:  0.99 
    - F1-score: 1.00 

- Label 1
    - Precision: 0.84 
    - Recall:  0.99
    - F1-score: 0.91



For the original logistic regression model, the results displayed high precision, recall, and f1-score for predicting the 0 label, which indicates healthy loans with 1.00, 0.99, and 1.00 scores respectively. For the 1 label, the model also has decent precision, recall and f1-score with 0.85, 0.91 and 0.88 scores respectively. However, it could be further evaluated with additional metrics and possibly tuned to improve its performance.

After taking a look into the logistic regression model with resampled training data, we were able to visualize a notable increase for label 1 on especially the recall and f1-score. Label 0 retained the near perfect scores displaying 1.00, 0.99, and 1.00 scores respectively. In label 1 we were able to see the recall jump from a 0.91 to a 0.99 as well as f1-score receiving a bump from 0.88 to 0.91. 

## Results Overview
Based on the evaluation results, we do recommend using the logistic regression model with resampled training data for predicting loan risks as it is more effective at distinguishing high-risk loans with high recall accuraccy. However, we should also consider the cost of false positives and false negatives in our recommendation, as well as potential biases in the data and model. It's important to continue monitoring and improving the model's performance over time to ensure its effectiveness and reliability.
