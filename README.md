# credit-risk-classification
In this repo you will find a folder Credict_Risk which contains the credit_risk_classification.ipynb file that includes the code used for the model.  In that folder you will also find a Resources folder that contains the lending_data.csv file used for the model. 

Below is the report for the analysis: 

## Overview of the Analysis


This analysis was conducted to help create a machine learning model to predict healthy and high-risk loans for a bank.  In order to create the model data from previous loans was provided which included loan_size, interest_rate, borrower_income, debt_to_income, num_of_accounts, derogatory_marks, total_debt and the loan_status.  For this analysis what we were trying to predict the loan_status (0: healthy loan, 1: high risk loan) which is our label by using the other variables as features.  In order to be able to create this model we first split the data that was provided into training (X_train, y_train) and testing (X_test, y_test) data. The next step was to create the model using logistic regression.  The model is then fit to the training data.  After fitting your model, you can make predictions and compare that to your testing data.  You then create your confusion matrix and print your classification report to see how well the model performed. 

## Results


Machine Learning Model(Logistic Regression): 
    * Accuracy: 0.99
    * Precision: 0.94
    * Recall: 0.84



## Summary
Although this model has a 99% accuracy I would be hesitant to recommend it without first determinining what the company is more interested in.  The reason is because the data that the model is trained on is 97% weighed towards healthy loans which means the model is weighed towards predicting loans as being good.  Due to this it is important to analyze the recall and precision values.  Recall means that out of every instance my model predicts a loan as being risky, 84% of those loans actually end up being risky loans.  Precision means that out of all the people who would have a risky loan the model catches 94% of those loans.  In order to potentially better the model it could be trained on dataset that was 50/50 between good and risky loans.  

