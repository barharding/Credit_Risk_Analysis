# Credit_Risk_Analysis

## Overview

The purpose of this analysis was to accurately predict low and high risk loans through the use of a machine learning model.  In this analysis six different models were trained and analyzed for their effectiveness.

# Results

For the six models below we use the balanced accuracy score to better judge the performance of our analysis where there is an imbalanced dataset meaning we have a great deal more low risk applicants then we do high risk applicants.  The sample dataset has 87 high risk applicants and 17118 low risk applicants.

By leveraging recall we can see how well the model was at predicting the right level of risk and precision tell us the degree of error in the categorization, i.e. what % of high risk applicants we categorized as low risk or what % of low risk applicants were deemed high risk.

- **Random OverSampler**
  - Balanced accuracy score 0.6456 indicates the model is not doing very well at predicting credit risk
  - The Precision & Recall scores for both High and Low risk are shown in figure 1 and like the balanced accuracy score does not really perform well. 
 

**_Figure 1: Random OverSampler Classification Report_**

![RandomOverSampler](/images/Naive_Random_Oversampling_Classification_Report.png)

- **SMOTE algorithms**
  - Balanced accuracy score 0.6564 indicates the model is not doing very well at predicting credit risk.
  - The Precision & Recall scores for both High and Low risk are shown in figure 2 and like the balanced accuracy score does not really perform well.

  **_Figure 2: Smote_**

![Smote](/images/Smote_Oversampling_Classification_Report.png)

- **Cluster Centroids algorithm**
  - Balanced accuracy score 0.5142 indicates the model is not doing very well at predicting credit risk.
  - The Precision & Recall scores for both High and Low risk are shown in figure 3.

  **_Figure 3: Cluster Centroids_**

![Cluster Centroids](/images/undersampling_Classification_Report.png)

- **Smoteenn**
  - Balanced accuracy score 0.6794 indicates the model is not doing very well at predicting credit risk.
  - The Precision & Recall scores for both High and Low risk are shown in figure 4 and like the balanced accuracy score does not really perform well.

  **_Figure 4: Smoteen_**

![Smoteenn](/images/combination_over_under_Classification_Report.png)

- **Balanced Random Forest Classifier**
  - Balanced accuracy score 0.7877 indicates the model is not doing very well at predicting credit risk.  While the accuracy percentage is higher than those above a look at the confusion matrix will show that 1560 low risk loans were false negatives a potential big loss of revenue.
  - The Precision & Recall scores for both High and Low risk are shown in figure 5 

  **_Figure 5: Balance Random Forest Classifier Classification Report & Confusion Matrix_**

![Balanced Random](/images/Balanced_Random_Forest_Classification_Report.png)

- **Easy Ensemble Classifier**
  - Balanced accuracy score 0.9254 indicates the model is doing very well at predicting credit risk.  That said it still catagorized 979 low risk as high.
  - The Precision & Recall scores for both High and Low risk are shown in figure 6
  
  **_Figure 6: Easy Ensemble Classifier Classification Report & Confusion Matrix_**

![Easy Ensemble](/images/Easy_Ensemble_Classification_Report.png)

## Summary

The credit risk analysis shows that none of the models perform well even the Easy Ensemble Classifier which has a high balanced accuracy score. The reason for rejecting all of them is because too many low risk loans were being categorized as high risk.  In addition, given the true volume of high risk loans being so small in comparison to the low risk volumne it is better to have a much higher recall and precision score on the low risk loans otherwise the loan company would lose too much revenue.  Additional models should be tested to see if there are better ones out there.

