# Module20

# Credit Risk Analysis Report

## Overview of the Analysis

The point of this exercise is to build a model to predict the status of loans (whether they are considered healthy or high-risk) using 7 features provided in the data set. The variables I was using to predict the status are: loan-size, interest rate, the borrower income (yearly), the ratio of the loan size divided by the borrower's yearly income (calculated from 2 other variables being used), number of accounts the borrower has, deragotory marks on the borrower's file, and total debt of the borrower. Logisitic regression was chosen as the method of regression, since we are looking at predicting a classification (healthy or high-risk) as opposed to a continuous variable we are trying to predict.  

## Results

* Logistic Learning Model:
  * The Healthy Loan Status predictions had a recall score of 1.00, and a precision score of 1.00. This leads to an f1-score of 1.00, as high of an f1-score you can see
  * The High-Risk Loan Status predictions had a recall score of 0.89, and a precision score of 0.87. This leads to an f1-score of 0.88. This is still a pretty high f1-score, but not nearly as strong as the score for healthy loan statuses.
 
## Summary

I would recommend using this model for identifying healthy loans, and flagging potential high-risk loans. The incredibly high scores of the healthy loan status classification indicate that when the model identifies a loan as healthy it is overwhelmingly unlikely for the classification to be a false positive. However, since there appears to be about a 10% chance that high-risk classified loans are false negatives, these loans should be reviewed further by human eyes and judgement. Still, these reviewed loans will come back as a high-risk determination far more often than not. 
