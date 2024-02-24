## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:
* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

The purpose of this analysis is find out the accuracy of the machine learing model to classify the loans issued by the lending company as healthy or high-risk loans. Features like borrower's income, debt to income ratio, total debt, interest rate, etc. are used to predict if the loan offered to the customer is a heathly loan or a high-risk loan.

Supervised machine learning approach is used to train the model to predict the loan outcomes with greater accuracy. A large subset of the labeled data is used to teach the model to recognize classification patterns of the loan - healthy or high-risk. In the next step, a smaller subset of labeled data is used test the model. Testing data helps understand how well the model is able to classify the loans correctly. 

Model is based on Logistic regression. It predicts the classification of the loan from customer data points like income, existing debts, etc


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.
* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.

                precision    recall  f1-score   support

  Healthy Loan       1.00      0.99      1.00     18765
High Risk Loan       0.85      0.91      0.88       619

      accuracy                           0.99     19384
     macro avg       0.92      0.95      0.94     19384
  weighted avg       0.99      0.99      0.99     19384

The model has a precision of 1.00 for healthy loans, indicating that it predicts healthy loans correctly 100% of the time. The model correctly identifies 99% of actual healthy loans (recall - 0.99).

The model predicts a loan as high-risk correctly 85% of the time and it correctly identifies 91% of actual high-risk loans (recall - 0.91).


## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

The model performs expectionally well for healthy loans. Heathly loans also constitute bigger portion of the total loans issued by the lending service company. A high precision, recall, and F1-score for healthy loans indicates very good predictive performance by the model for healthy loans. 

For predicting high-risk loans, model does a good job with good precision, recall and F1-scores. I would recommend that this model can be used to predict classification of loans issued by the lending company for future loans.

It is important to predict both classes of loan with greater accuracy. Because the company will make more profit by issuing more healthy loan and cut its losses by issuing less high-risk loans. So both classification are important for overall growth of the company.