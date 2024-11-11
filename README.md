# credit-risk-classification
* In this Challenge, I used various techniques to train and evaluate a model based on loan risk using a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

* This Challenge are divided into the following subsections:

    * Split the Data into Training and Testing Sets
    * Create a Logistic Regression Model with the Original Data
    * Write a Credit Risk Analysis Report

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

4. Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?

# Step 3: Write a Credit Risk Analysis Report

* Write a brief report that includes a summary and analysis of the performance of the machine learning models that was used. 

    * An overview of the analysis: Explain the purpose of this analysis.

    * The results: Using a bulleted list, describe the accuracy score, the precision score, and recall score of the machine learning model.

    * A summary: Summarize the results from the machine learning model. Include the justification for recommending the model for use by the company. If you don’t recommend the model, justify your reasoning.