# Supervised Machine Learning Report Template

## Overview of the Analysis

**Purpose:**

The Purpose of this analysis was to create a prediction model, which can be utilized to analyze credit worthiness of borrowers for the bank to putline any potential defaults.

The dataset provided contained just over 77,500 entried with specific indicators which are: Loan Size, Interest Rate,  Borrower's Income,  Number of regular payments for Borrower ,Detrimental factors on credit reportsand finally Borrowers total debt.

Within the dataset 3.2% of the total loans are in default. This was determined looking into the Loan Status columnn. The total value of loans amounted to over $760 Million, with over $46 Million. Default loans account for 6.08%, which when comapred to the total value could be seen as reasonable loss, however the bank has a duty to shareholders to reduce the amount wherever possible.

Initial steps involved removing the loan status column and storing in a seperate DataFrame, furthering on data features were split into training/ testing data, with a 75/25% split. Training Data was used in a Logistrical Regression model, resulting in a sctore of 0.99212 and testing score of 0.99184 which was used to predict test data and indiactors generated for balanced accuracy score, confusion matrix and class report.

Testing data then underwent random oversampling of the loan default status, with the purpose being to over-represent default loans to test the models predictive capabilities, the resulting data was composed of equal points for both healthy (0) and default(1) loans. A model was fit using Logistrical regression for resampled data which was then used to test Original data again. Further anlaysis was done on the feature data using StandardScalar, this prediction model yielded higher accruacy results than using raw data. Balanced accuracy increased by .379, precision dropped by 1% with recall incresing by 7%. The confusion matrix demonstrated a drop in false positives however false negatives did also increase. 

Therefore although the oversampled scaled data was accurate to 99% it demonstrated insignificant improvement over the use of raw data with the numbers being very similar, due to the drastic increase in false negatives rising, my recommendation would have been to continue using raw data when predicting.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
