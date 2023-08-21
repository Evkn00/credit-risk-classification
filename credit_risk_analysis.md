# Module 12 Report Template

# credit-risk-classification

## An overview of the analysis:
This analysis uses the lending_data.csv dataset which contains loan information on borrowers and identifies their likelyhood to default on loan repayments.
The dataset includes over 77,000 rows of deidentified loan data, each of which has the following features:
- loan_size
- interest_rate
- borrower_income
- debt_to_income
- num_of_accounts
- derogatory_marks
- total_debt
- loan_status

The loan status can be either a 0 meaning the loan is healthy with low risk of default, and a 1 being an unhealthy loan with a high default risk. 

The analysis takes the form of supervised machine learning using a classification algorythm featuring linear regression to predict whether loans are likely to default. The dataset is split randomly into a training dataset to help the algorythm learn about what features are contributing factors to whether a loan is likely to default and then the remaining part of the data set is used to test the algorythm for accuracy and whether it is likely to be useable in a real-world scenario. 

## The results
Three scores help us to understand how effective the model will be. For this model the scores were:

Accuracy: 0.99 very high accuracy score overall is good. 

Precision:
An F1 score of 1.00 for low-risk loans is very high.
An F1 score of 0.88 for high-risk loans is still reasonably high, but there is an element of risk involved, so further parameter tuning should be undertaken.

Recall: for healthy loans the recall score is 0.99, for high-risk loans the recall score is 0.91. Once again this could likely be rectified with parameter tuning. 

## The summary
As this model is being used to assess the risk of default on loans, I would not recommend using until the parameters have been tuned to attempt to get higher recall and f1 score for high risk loans. While 0.88 and 0.91 are quite high, when dealing with an model that may be used to take on risk by the bank and take on risk by customers, higher accuracy is definetly desirable. A determination of the level of recall and F1 required should be undertaken, however I would suggest aiming for 0.95 as the target for both before implementing the model. 
