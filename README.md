# credit-risk-classification
Credit-risk-classification Challenge related files are in the repository

# Solution
There is one folder called Credit_Risk in which you will find the file with the code and analysis report and the Resources folder.

## Background
In this Challenge, you’ll use various techniques to train and evaluate a model based on loan risk. You’ll use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

## Instructions
The instructions for this Challenge are divided into the following subsections:

Split the Data into Training and Testing Sets

Create a Logistic Regression Model with the Original Data

Write a Credit Risk Analysis Report

Split the Data into Training and Testing Sets
Open the starter code notebook and use it to complete the following steps:

Read the lending_data.csv data from the Resources folder into a Pandas DataFrame.

Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.

NOTE
A value of 0 in the “loan_status” column means that the loan is healthy. A value of 1 means that the loan has a high risk of defaulting.

Split the data into training and testing datasets by using train_test_split.

Create a Logistic Regression Model with the Original Data
Use your knowledge of logistic regression to complete the following steps:

Fit a logistic regression model by using the training data (X_train and y_train).

Save the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.

Evaluate the model’s performance by doing the following:

Generate a confusion matrix.

Print the classification report.

Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?

Write a Credit Risk Analysis Report
Write a brief report that includes a summary and analysis of the performance of the machine learning models that you used in this homework. You should write this report as the README.md file included in your GitHub repository.

Structure your report by using the report template that Starter_Code.zip includes, ensuring that it contains the following:

An overview of the analysis: Explain the purpose of this analysis.

The results: Using a bulleted list, describe the accuracy score, the precision score, and recall score of the machine learning model.

A summary: Summarize the results from the machine learning model. Include your justification for recommending the model for use by the company. If you don’t recommend the model, justify your reasoning.


## Credit Risk Analysis Report

### Overview of the Analysis

An analysis was done to develop machine learning model to predict loan status based on various financial features. The data provided included loan_size, interest_rate, borrower_income, debt_to_income, num_of_accounts, derogatory_marks, total_debt, and loan_status. The task of the machine learning model was to predict whether a loan is healthy (0) or high-risk loan (1). 

We went through multiple stages of the Machine Learning Process. First was data preparation, which is was preprocessed by separating features and labels, and then split into training and testing sets. Then logistic regression was chosen as the primary model due to its simplicity and interpretability. After, the Logistic Regression model was trained using the training data. Lastly, the trained model was evaluated on the testing data using metrics such as accuracy, precision, and recall.

### Results

Loan_status:
- Healthy loan (0): 18,759 instances
- High-risk loan (1): 625 instances

Machine Learning Model 1:
- Accuracy: 99%
- Precision (Healthy Loan): 100%
- Recall (Healthy Loan): 100%
- Precision (High-risk Loan): 87%
- Recall (High-risk Loan): 89%

### Summary

The logistic regression model performed remarkably well in predicting both healthy and high-risk loans. It achieved perfect precision and recall for healthy loans, indicating that it accurately identified all healthy loans without misclassification. As for high-risk loans, although the precision and recall scores were slightly lower, the model still demonstrated strong performance, correctly identifying a significant portion of high-risk loans.

The importance of prediction may depend on the problem at hand. For instance, if the focus is on minimizing the risk associated with high-risk loans, then predicting high-risk loans (1) accurately becomes crucial. However, the model's ability to accurately predict healthy loans (0) is also essential to ensure that low-risk opportunities are not missed. Thus, a balanced approach in predicting both classes is necessary. The logistic regression model demonstrates strong performance and is well-suited for the task of loan classification in this context.

