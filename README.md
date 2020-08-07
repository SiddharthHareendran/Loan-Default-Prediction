# Loan-Default-Prediction

Loan default is the failure to repay a loan according to the terms agreed to in the promissory note. A lender may take legal action to get the money back.
The objective of this Model is to predict if a loan will default or not.

Features considered:
1) Loan Amount
2) Term
3) Credit Score
4) Annual Income
5) Years in Current Job
6) Home Ownership status
7) Purpose of Loan
8) Monthly EMI
9) Years of Credit History
10) Months Since Last Delinquency 
11) Number of Open Accounts
12) Number of Credit Problems
13) Current Credit Balance
14) Bankruptcy in past

# Scoring : Fbeta
Fbeta is the Harmonic Mean of Recall and Precision.
The objective of this Model is to predict if a loan will default or not. Objectives of Banks is to give out as much loan out as possible with out those loans going bad since interest rate on loan is how banks make a profit. Hence the priority of the model is to detect correctly if a Loan will go bad as against a good loan. Hence the model has to correctly identify that a loan will go bad(i.e. 1) at the same time not penalise good customers and wrongly identifing them as defaulters. If good customers are also wrongly identified, bank loses out on a business opportunity. Hence these false positives are given more weightage and hence the very low(<1) beta score. Also due to the imbalanced nature of the data set, fbeta score gives us a result between precision and recall. Hence the chosen metric is Fbeta Score.

# Performance
Best Model: Decision Tree Classifier
Best Mean Cross Validation Score is 0.864
Best Mean Cross Validation params is {'class_weight': {0: 10, 1: 1}, 'max_depth': 4, 'splitter': 'random'}
Train score is 0.866
Test score is 0.853
