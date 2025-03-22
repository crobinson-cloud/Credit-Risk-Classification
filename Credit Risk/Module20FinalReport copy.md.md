# Module 20 Report  (CR)

## Overview of the Analysis

1. Explain the purpose of the analysis
A: The purpose of the analysis is to determine if the Logistic Regression Machine Learning Model can more accurately predict healthy vs high-risk loans, using the original dataset that s resampled to increase the size of the minority class.
2.  Explain what financial information the data was on, and what you needed to predict.
A: The data consisted of 77,536 loans that included columns for loan_size, interest_rate, borrower_income, debt_to_income_ratio, number_of_accounts, derogatory_marks, total_debt, and loan_status. The category we are attempting to predict with this analysis is "loan_status". The data in the remaining columns will be used as features to train the data and inform predictions. 

3. Describe the stages of the machine learning process you went through as part of this analysis.
A:  The stages of machine learning process are as follows: 
- prepare the data - import the file, establish dataframe, evaluate columns and features
- separate the data into features and labels- labels your are attempting to predict, is the loan status healthy (0) or high-risk (1)
- Use train test split function to separate the features and labels data into training and testing datasets.
- import the machine learning model from the library (using LogisticRegression from SKLearn)
- Instantiate the model
- Fit the model using training data
- Use the model to make predictions using the features test data
- Evaluate predictions

4. Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
A: Primary model used in this analysis: LogisticRegression from SKLearn
Supporting functions: train_test_split from SKLearn
Models Evaluated using: confusion_matrix from SKLearn and classification_report from SKLearn

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model: Logistic Regression
- **Accuracy score:** 99%
- **Precision Score:** 
	- Class 0 (healthy loans)-100%
	- Class 1 (high-risk loans)- 84%
-**Recall Scores:**
	- Class 0 (healthy loans) - 99%
	- Class 1 (high-risk loans) - 94 %
  

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any.
A: It does very well with using the original data to predict healthy loan values. Precision is at 100%, while recall is at 99%. It was not as good prediciting high risk loan values, with precision at 84% and recall at 94%.

The Logistic Regression model works well, however I would also see if there are other models it could perform better on.

