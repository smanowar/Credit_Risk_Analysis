# Credit_Risk_Analysis

## Overview

The purpose of this analysis is to predict the status of loan applications using various algorithms from the imbalanced-learn and scikit-learn libraries including: 
- Oversampling Methods (Naive Random Oversampling, SMOTE Oversampling)
- Undersampling Methods (Cluster Centroids)
- Combonation Methods (SMOTEEN)
- and Ensemble Learners (Balanced Random Forest Classifier, and Easy Ensemble Classifier)
 
Data was taken from *LoanStats_2019Q1.csv*, and analysis was performed using Jupyter Notebook.

## Results
Using Jupyter Notebook, analysis for the six different algorithms were calculated below. Results were rounded to two decimal places.

### Oversampling Methods

***Naive Random Oversampling***<br>

Our results from Jupyter Notebook were as follows:
<p align="left"><img src=https://github.com/smanowar/Credit_Risk_Analysis/blob/main/images/naive_random_sampling.PNG?raw=true> </p>

In summary, the results for the naive random oversampling method are:
- Balanced Accuracy Score: 54%
- Precision: 99%
- Recall: 40%

<br>***SMOTE Oversampling***<br>

Using Jupyter Notebook, the results are as follows:
<p align="left"><img src=https://github.com/smanowar/Credit_Risk_Analysis/blob/main/images/SMOTE.PNG?raw=true></p> 

In summary, the results for the SMOTE method are:
- Balanced Accuracy Score: 65%
- Precision: 99%
- Recall: 68%
<br><br>
### Undersampling Methods

***Cluster Centroids***<br>

The results from Jupyter Notebook are as follows:
<p align="left"><img src=https://github.com/smanowar/Credit_Risk_Analysis/blob/main/images/undersampling.PNG?raw=true> </p>

In summary, the results for the undersampling method are:
- Balanced Accuracy Score 54%
- Precision: 99%
- Recall: 40%
<br><br>
### Combonation Methods

***SMOTEEN***<br> 

The results from Jupyter Notebook are as follows:
<p align="left"><img src=https://github.com/smanowar/Credit_Risk_Analysis/blob/main/images/SMOTEEN.PNG?raw=true></p>

In summary, the results for the SMOTEEN method are:
- Balanced Accuracy Score: 64%
- Precision: 99% 
- Recall: 57%
<br><br>
### Ensemble Learners

***Balanced Random Forest Classifier***<br>

The results from Jupyter Notebook are as follows:
<p align="left">
<img src=https://github.com/smanowar/Credit_Risk_Analysis/blob/main/images/random_forest.PNG?raw=true> 
</p>

In summary, the results for the Balanced Forest Classifier method are:
- Balanced Accuracy Score: 79%
- Precision: 99%
- Recall: 91%

<br>***Easy Ensemble Classifier***<br>

The results from Jupyter Notebook are as follows:
<p align="left">
<img src=https://github.com/smanowar/Credit_Risk_Analysis/blob/main/images/easy_ensemble.PNG?raw=true> 
</p>

In summary, the results for the Easy Ensemble Classifier method are:
- Balanced Accuracy Score: 93%
- Precision: 99%
- Recall: 94%

## Summary
The overall goal of the bank is to minimize the amount of clients that default on their credit product. Therefore, it would be preferrable that a low-risk client is denied (a false negative) versus that situation a high-risk client is approved (false positive). Based on this the metric we would use to analyze the models would be precision.

All the models show weak precision in determining if the client is high-risk. The large amounts of false negatives that each of the models produces would work against the bank's interest, as it would:

1. miss out on revenue from the declined applications of low-risk clients
2. hurt their reputation as a lender - because they would be declining a huge amount of applicants (a large amount of those who are falsley categorized as high-risk clients), they could gain a bad reputation with potential clients which could hurt their lending strategy in the long run. 
