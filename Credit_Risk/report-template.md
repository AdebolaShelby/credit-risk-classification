# Overview of the Analysis

The purpose of this analysis is to develop a supervised machine learning model that predicts whether a loan is classified as healthy (class 0) or high-risk (class 1). We will utilize logistic regression as our binary classification method. The analysis focuses on financial data, specifically examining factors such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. Our objective is to determine the loan status, categorizing it as either a healthy loan (0) or a high-risk loan (1).


# Step 1: Split the Data into Training and Testing Sets

1. Read the lending_data.csv data from the Resources folder into a Pandas DataFrame.

2. Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.

3. Split the data into training and testing datasets by using train_test_split.

# Step 2: Create a Logistic Regression Model with the Original Data

1. Fit a logistic regression model by using the training data (X_train and y_train).

2. Save the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.

3. Evaluate the model’s performance by doing the following:

    * Generate a confusion matrix.

    * Print the classification report.

## Results

* Logistic Regression Model Accuracy, Precision, and Recall scores.

    * Accuracy: The overall accuracy of the model is 0.99, indicating that it correctly classifies 99% of the instances.

    * Precision

        * Healthy Loan (class 0): 1.00
        * High-Risk Loan (class 1): 0.85
    * Recall

        * Healthy Loan (class 0): 0.99
        * High-Risk Loan (class 1): 0.95

## Summary

The logistic regression model performs very well in predicting healthy loans (class 0), achieving a precision of 1.00 and a recall of 0.99. In contrast, the model's performance for risky loans (class 1) is still solid, with a precision of 0.85 and a recall of 0.95.

The lower precision and recall for predicting risky loans can be attributed to our imbalanced dataset; the support for class 1 consists of only 619 instances, which is significantly lower compared to the support for class 0. This lack of data points for high-risk loans limits the model's ability to learn effectively. To improve predictions for high-risk loans, it would be beneficial to include more examples of this type in the training dataset.

In the context of loan classification, preventing high-risk loans is paramount, since the potential losses from a single default can outweigh the interest earned from numerous successful loans. Overall, the model achieves a high total accuracy of 99%.
