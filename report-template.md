# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
    The purpose of this analysis was to use historical lending data to evaluate the whether a potential loan is low-risk or high-risk.
* Explain what financial information the data was on, and what you needed to predict.
    The financial information included loan size, interest rate, borrower income,debt to income, number of accounts, derogatory marks, total debt, and loan status. We were predicting loan status.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
    The loan status column had only two potential varaibles: 0 (healthy loans) and 1 (high-risk loans)
* Describe the stages of the machine learning process you went through as part of this analysis.
    First the data was split into training and testing sets to evaluate the model on unseen data. Then a logistic regression model was selected because the focus data was binary, and the model was trained. Finally, the model's performance was evaluted by calculating its precision, recall, and f1-score values.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).
    The logistic regression method was chosen because it's ideal for working with binary data.

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.
        - Accuracy = 0.99 --The model achieved an overall accuracy of 99%, indicating that it correctly classified 99% of the loans in the dataset.
        - Precision(0) = 1.00 --100% of the loans predicted as healthy were, in fact, healthy.
        - Recall (0) = 0.99 --The model correctly identified 99% of all actual healthy loans.
        - F-1 score (0) = 1.00 --Indicates a perfect balance between precision and recall for healthy loans.
        - Precision (1) = 0.85 --85% of the loans predicted as high-risk were, in fact, high-risk.
        - Recall (1) = 0.91 --The model correctly identified 91% of all actual high-risk loans.
        - F-1 score (1) = Indicates a good, but not perfect balance between precision and recall for high-risk loans.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
    The logistic regression model performed the best. I know it performed the best because it received an accuracy score of 99%.
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
    Yes. Healthy loan predictions are more accurate than high-risk loan predictions. This is inconvenient because mistaking a high-risk loan for a healhty loan can result in granting a loan that will never be paid back. It's, therefor, more important to predict the high-risk loans.

If you do not recommend any of the models, please justify your reasoning.
    No.
