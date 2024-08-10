# Credit Risk Classification Report

## Overview of the Analysis
* The purpose of the analysis:
  - The purpose of this analysis was to see if we can more accurately predict healthy loans versus high-risk loans by using a Logistic Regression machine learning model, The objective was to predict the loan status, either as a healthy loan (0) or a high-risk loan (1). The data used is a 77,536 loan data CSV file.

* Explain what financial information the data was on, and what you needed to predict:
  - The analysis was conducted on financial data, specifically focusing on loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The objective was to predict the loan status, either as a healthy loan (0) or a high-risk loan (1). The data used is a 77,500-line CSV file.

* The stages of the machine learning process in this analysis included:
  - In order to get clean, useful data, it had to be prepared by importing the data from the source, and converting to a dataFrame, to be evaluated.
  - Split the data into labels and features, with the loan status (healthy or high-risk) being the label and the remaining seven columns as features.
  - The data was then split into training and testing data sets by using the split function.
  - A Logistic Regression model from sklearn was created. and classified as a binary classifier because only healthy or high-risk were our only two options.
  - The model was instantiated, then fit with the training data, and predictions were made with the test data.
  - The model's performance was evaluated by generating a confusion matrix, classification reports, and accuracy scores, then compared with each other.
* The Machine Learning methods that were used
  - The primary model used in this analysis for the LogisticRegression model was from SKLearn.
  = The supporting functions that were used in this analysis were train_test_split from SKLearn.
  - The models were evaluated using the confustion_matrix from SKLearn, and the classification_report from SKLearn.

## Results

* Logistic Regression:
    * Testing Set:

        - Accuracy: 99%
        - Precision Label 0 - Healthy Loan: 100%
        - Precision Label 1 - High-risk Loan): 84%
        - Recall Label 0 - Healthy Loan): 99%        
        - Recall Label 1 - High-risk Loan): 94%

## Summary

Our logistic regression model was correct almost every time in predicting the 0 class (healthy loans), with 100% precision, and 99% recall was almost as correct. With the risky loans (class 1), it had slightly lower percentages, but the model still did well with a good prediction of 84% precision and 94% recall.

Overall, this logistic regression model was quite effective. with results for both testing and training displaying 99% accuracy. But there would be a need to test with a number of different data sets to assure that the numbers are more accurate, before we use this logistic regression model completely.
