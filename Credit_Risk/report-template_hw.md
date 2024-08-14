# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
    The purpose of the analysis is to build a model that is based on historical lending activity that can identify the creditworthiness of borrowers. 0 representing that a client has a healthy credit while 1 represents a risky credit.
* Explain what financial information the data was on, and what you needed to predict.
    The historical data that was given had information of the loan size, interest rate,	borrower income, debt to income, number of accounts, derogatory marks, and total debt. based off these factors the model will predict if the loan is healthy or at risk. I'm assuming healthy in the sense that it will be okay for the financial institution to lend money to the client at the loan size, interest and interest rate given the borroer's income, debt to income ratio, etc.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
    In the data there are 19,384 loans that were fed into the model and 99.2% (18,679 + 558/ 19,384) were accurately predicted by the model.
* Describe the stages of the machine learning process you went through as part of this analysis.
    The data was first split between the training data and the test data. A logistic regression model was called with a random state of 1 and the training data was fit to it. Test data was ran through that model and the predictions that came out were stored. The original data and the predictions were put into the confusion matrix and a classification report from the model was generated.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).
    

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
