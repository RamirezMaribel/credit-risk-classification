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
    I think the best method for this case was the logistic regression as we wanted to both train the model and test the model on the actual data that was provided. I believe using a regression model might not be as accurate as it's seems to only be a two dimensional model where as the data that was given had many dimensions. I think a decision tree model or random forest model would also work with this type of data, but I believe that sectioning off some dimensions to determine if the loans are healthy or risky could lead to lower precision and recall rates.
    

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.
    -Accuracy of the model showed an F-1 score of 99%
    -Precision of 0-healthy showed 100%, 1-risky showed 87%
    -Recall of 0-healthy showed 100%, 1-risky showed 89%

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best? 
    I don't know that any one test performs the best. From what I understand efficency; we want the model to learn and predict results accurately so that manual computation won't be necessary and won't take as long. We could use all methods that we've learned and I believe the results will be close to each other. I would recommend trying not only the logistic regression but also random forest and maybe KNN. I think Random Forests might also help in seeing which factors contribute the outcome and could help in requesting more specific information that may make it easier for future machine learning. I also believe that KNN might also show this as users with healthy or even risky scores tend to have near the same habits and that itself is stored historical data.
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
    Performance of the model depends on the situation. In this case, I believe that predicting the 1's (risky) is mroe important. No one wants to lend money to someone with a risky history or show current risk in the financials they have. History tends to repeat itself which is why I think supervised learning is advantagous not only in the financial world, but also in many other business aspects. In other cases, maybe the 0 (healthy) would be more sought out; say the institution would like to send out a promotion to those with healthy financial standing. You'd definitely want to lend money to people who have previously shown responsible and accountable consistent financing.

If you do not recommend any of the models, please justify your reasoning.
