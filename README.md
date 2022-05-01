# Credit_Risk_Analysis

## Overview

Explain the purpose of this analysis.

# Results

For the six models below we use the balanced accuracy score to better judge the performance of our analysis where there is an imbalanced dataset meaning we have a great deal more low risk applicants then we do high risk applicants.

By leveraging recall we can see how well the model was at predicting the right level of risk and precision tell us the degree of error in the categorization, i.e. what % of high risk applicants we categorized as low risk or what % of low risk applicants were deemed high risk.

- RandomOverSampler
  - Balanced accuracy score 0.6456 indicates the model is not doing very well at predicting credit risk
  - The Precision & Recall scores for both High and Low risk are shown in figure 1 and like the balanced accuracy score does not really perform well. 
 

**_Figure 1: Random OverSampler Classification Report_**

![RandomOverSampler](/images/Naive_Random_Oversampling_Classification_Report.png)

- SMOTE algorithms
  - Balanced accuracy score 0.6564 indicates the model is not doing very well at predicting credit risk
  - The Precision & Recall scores for both High and Low risk are shown in figure 2

  **_Figure 2: Smote_**

![Smote](/images/Smote_Oversampling_Classification_Report.png)

- ClusterCentroids algorithm
  - Balanced accuracy score 0.5142 indicates the model is not doing very well at predicting credit risk
  - The Precision & Recall scores for both High and Low risk are shown in figure 3

  **_Figure 3: Cluster Centroids_**

![Cluster Centroids](/images/undersampling_Classification_Report.png)

- Smoteenn
  - Balanced accuracy score 0.6794 indicates the model is not doing very well at predicting credit risk
  - The Precision & Recall scores for both High and Low risk are shown in figure 4

  **_Figure 4: Smoteen_**

![Smoteenn](/images/combination_over_under_Classification_Report.png)

- BalancedRandomForestClassifier
  - Balanced accuracy score 0.7877 indicates the model is not doing very well at predicting credit risk
  - The Precision & Recall scores for both High and Low risk are shown in figure 5

  **_Figure 5: Balance Random Forest Classifier Classification Report_**

![Balanced Random](/images/Balanced_Random_Forest_Classification_Report.png)

- EasyEnsembleClassifier
  - Balanced accuracy score 0.9254 indicates the model is doing very well at predicting credit risk
  - The Precision & Recall scores for both High and Low risk are shown in figure 6
  
  **_Figure 6: Easy Ensemble Classifier Classification Report_**

![Easy Ensemble](/images/Easy_Ensemble_Classification_Report.png)

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.

There is a summary of the results (2 pt)
There is a recommendation on which model to use, or there is no recommendation with a justification (3 pt)

