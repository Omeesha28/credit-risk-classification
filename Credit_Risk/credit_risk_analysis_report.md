# Module 12 Report

## Overview of the Analysis

An analysis was done to develop machine learning model to predict loan status based on various financial features. The data provided included loan_size, interest_rate, borrower_income, debt_to_income, num_of_accounts, derogatory_marks, total_debt, and loan_status. The task of the machine learning model was to predict whether a loan is healthy (0) or high-risk loan (1). 

We went through multiple stages of the Machine Learning Process. First was data preparation, which is was preprocessed by separating features and labels, and then split into training and testing sets. Then logistic regression was chosen as the primary model due to its simplicity and interpretability. After, the Logistic Regression model was trained using the training data. Lastly, the trained model was evaluated on the testing data using metrics such as accuracy, precision, and recall.

## Results

Loan_status:
- Healthy loan (0): 18,759 instances
- High-risk loan (1): 625 instances

Machine Learning Model 1:
- Accuracy: 99%
- Precision (Healthy Loan): 100%
- Recall (Healthy Loan): 100%
- Precision (High-risk Loan): 87%
- Recall (High-risk Loan): 89%

## Summary

The logistic regression model performed remarkably well in predicting both healthy and high-risk loans. It achieved perfect precision and recall for healthy loans, indicating that it accurately identified all healthy loans without misclassification. As for high-risk loans, although the precision and recall scores were slightly lower, the model still demonstrated strong performance, correctly identifying a significant portion of high-risk loans.

The importance of prediction may depend on the problem at hand. For instance, if the focus is on minimizing the risk associated with high-risk loans, then predicting high-risk loans (1) accurately becomes crucial. However, the model's ability to accurately predict healthy loans (0) is also essential to ensure that low-risk opportunities are not missed. Thus, a balanced approach in predicting both classes is necessary. The logistic regression model demonstrates strong performance and is well-suited for the task of loan classification in this context.
