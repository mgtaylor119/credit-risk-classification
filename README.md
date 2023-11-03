# credit-risk-classification

## Overview of the Analysis

The objective of this analysis is to train and evaluate a machine learning model to assess loan risk. The dataset, lending_data.csv, encompasses historical lending data from a peer-to-peer lending services company. It includes various features such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, total debt, and loan status.

The primary aim is to predict the likelihood of a loan being at high risk based on the provided information. To accomplish this task, the following methods were employed:

1. **Train-Test Split:**
   - The dataset was divided into training and testing sets to facilitate model training and evaluation.

2. **Random Over-sampling:**
   - RandomOverSampler was applied to address class imbalance in the target variable, ensuring a balanced representation of high-risk and low-risk loans.

3. **Logistic Regression:**
   - The Logistic Regression algorithm was utilized for its effectiveness in binary classification tasks, making it well-suited for predicting loan risk.

By combining these techniques, the analysis aims to create a robust model for assessing loan risk based on the provided financial information.



## Results
* Machine Learning Model 1:
  * Accuracy Score: 99%
  * Precision Score: 0(healthy loan)- 100%, 1(high risk loan)- 87%
  * Recall Score: 0-healthy loan)- 100%, 1(high risk loan)- 89%

* Machine Learning Model 2:
  * Accuracy Score: 99%
  * Precision Score: 0(healthy loan)- 99%, 1(high risk loan)- 99%
  * Recall Score: 0-healthy loan)- 99%, 1(high risk loan)- 99%

## Summary

Both Machine Learning Model 1 and Model 2 demonstrate very high accuracy scores of 99%. This indicates that the models are performing exceptionally well in classifying loans.

In terms of precision, Model 2 shows high precision for both classes (0 and 1) at 99%. This means that when Model 2 predicts a loan as either healthy or high risk, it is highly accurate.

Similarly, Model 1 also shows high precision for class 0 (healthy loan) at 100%, indicating that when Model 1 predicts a loan as healthy, it is almost always correct. However, the precision for class 1 (high risk loan) is slightly lower at 87%, which means that there may be a small number of false positives for high-risk loans.

Both models have high recall scores for both classes (0 and 1) at 99% or above. This means that they are able to identify a high proportion of true positives for both healthy and high-risk loans.

In conclusion, both models perform exceptionally well in this scenario. However, Model 2 slightly edges out Model 1 in terms of precision for high-risk loans. Depending on the specific goals and requirements of the analysis, Model 2 might be the preferred choice due to its slightly higher precision. However, it's essential to consider other factors such as computational resources, interpretability, and business context before making a final decision.
