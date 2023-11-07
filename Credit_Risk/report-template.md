# Module 12 Report Template

## Overview of the Analysis

The analysis aimed to assess the performance of two logistic regression machine learning models in predicting credit risk associated with loans. The dataset consisted of historical lending data from a peer-to-peer lending services company, and the goal was to classify loans into low-risk (0) or high-risk (1) categories. 

The analysis involved the following key steps:

1.	Data Splitting: The dataset, comprising 77,536 data points, was split into training and testing sets.
2.	Model 1 (Original Data): The first logistic regression model (Logistic Regression Model 1) was built using the original data. Model 1 was then applied to the testing dataset, and its performance was evaluated.
3.	Class Imbalance Correction: The original dataset had a significant class imbalance, with 75,036 low-risk loans and only 2,500 high-risk loans. To address this, the training data was resampled using the RandomOverSampler module, resulting in 56,277 data points for both low-risk and high-risk loans.
4.	Model 2 (Resampled Data): A new logistic regression model (Logistic Regression Model 2) was constructed using the resampled data, and its performance was assessed.


## Results and factors considered:

Key factors considered in the analysis included loan size, interest rate, borrower's income, debt-to-income ratio, number of accounts, derogatory marks, and total debt.
The results of the analysis for both models are summarized as follows:


# Machine Learning Model 1: Logistic Regression with Original Data
•	Accuracy: 94%
•	Precision: 93% (with a 100% precision for low-risk loans but 87% precision for high-risk loans)
•	Recall: 95% (with a 100% recall for low-risk loans but 89% recall for high-risk loans)

In summary, Model 1 had strong performance in identifying low-risk loans with high precision and recall. However, it was slightly less effective in predicting high-risk loans, with a moderate level of precision and recall for this category.


# Machine Learning Model 2: Logistic Regression with Resampled Data
•	Accuracy: 99%
•	Precision: 93% (with a 100% precision for low-risk loans but 87% precision for high-risk loans)
•	Recall: 100%

Model 2, trained with resampled data, demonstrated superior accuracy, precision, and recall for high-risk loans compared to Model 1. While its performance for low-risk loans remained consistent, it showed a notable improvement in identifying high-risk loans.

## Summary

In conclusion, the analysis suggests that Logistic Regression Model 2, trained with resampled data, is the preferred choice for credit risk analysis. This model offers significant improvements in predicting high-risk loans, which is essential for minimizing potential financial losses for the lending company. Despite a slightly higher number of false positives for Model 2, its high accuracy and recall make it the more reliable option for assessing loan applications and mitigating credit risk.

The recommendation is to use Logistic Regression Model 2 for credit risk analysis, as it surpasses Model 1 in predicting high-risk loans, making it the better choice for assessing loan applications and making informed lending decisions. However, it's essential to note that neither model achieved precision above 90%, suggesting that further refinements may be needed to enhance credit risk prediction. Nevertheless, Model 2 outperforms Model 1 in terms of accuracy and recall and is, therefore, the model of choice for this specific analysis.


