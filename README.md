# Credit_Risk_Analysis

## OVERVIEW

For this project, Python was used to create and assess several machine learning models in order to predict credit risk. The data was obtained from LendingClub, a lending-services company, and contains over `68,000` usable entries. Data pertaining to credit risk is notoriously unbalanced, as good loans generally outnumber risky ones, and it was no different in this instance:

![alt_text](https://github.com/farwaali08/Credit_Risk_Analysis/blob/998b47f32893cbcf5e5951bc4f0605464546b270/Images/1.png)

The data was resampled using the different methods outlined below, and then each method was evaluated based on its performance.



| **Oversampling** | **Undersampling**|**Both**         |**Ensemble Methods**          |
|----------------- | -----------------|-----------------|-----------------             |
| RandomOverSampler| ClusterCentroids |SMOTEEN          |BalancedRandomForestClassifier|               
| SMOTE            |                  |                 |EasyEnsembleClassifier        |


**Note**: the ensemble methods are machine learning models that reduce bias by [generating under-sampled subsets combined inside an ensemble](https://imbalanced-learn.org/stable/references/ensemble.html). **EasyEnsembleClassifier** is a boosting algorithm, and **BalancedRandomForestClassifier** is a bagging algorithm.

## TOOLS & RESOURCES

#### Data
* LoanStats_2019Q1.csv

#### Software
* Python 3.9.3
  * Scikit-learn 
  * Imbalanced-learn 
* Jupyter Notebook 6.3.0
* Machine learning algorithms
  * RandomOverSampler
  * SMOTE
  * ClusterCentroids
  * SMOTEENN
  * BalancedRandomForestClassifier
  * EasyEnsembleClassifier 

## RESULTS & SUMMARY

### RandomOverSampler 

![alt_text](https://github.com/farwaali08/Credit_Risk_Analysis/blob/510252005f955af1904c3dc4b0f5246c65604689/Images/ROS.png)

   * Balanced accuracy test (appox.): `65%`
   * Precision: `1%`
   * Recall/Sensitivity: `61%`
   * F1: `2%`
   * Compared to the other models, this method fell somewhere in the middle. The overall balanced accuracy test score was approximately `65%`, and both precision and F-scores for high-risk prediction are low. The recall/sensitivity is moderate at `61%`.

### SMOTE

![alt_text](https://github.com/farwaali08/Credit_Risk_Analysis/blob/f2aaa4be14a5c2a278e534a08cb5e9b0335bf775/Images/SMOTE.jpg)

   * Balanced accuracy test (appox.): `62%`
   * Precision: `1%`
   * Recall/Sensitivity: `61%`
   * F1: `2%`
   * This model fared similarly to the previous one, with identical precision and F-scores. The recall/sensitivity is also identical, at `61%`. The overall balanced accuracy test score however, is lower, at roughly `62%`

### ClusterCentroids

![alt_text](https://github.com/farwaali08/Credit_Risk_Analysis/blob/340b32383dabea0fb75f48dfddbca7af1016a970/Images/Cluster.jpg)

   * Balanced accuracy test (appox.): `51%`
   * Precision: `1%`
   * Recall/Sensitivity: `60%`
   * F1: `1%`
   * This model was the least successful in predicting credit risk amongst all the models tested. It produced the lowest balanced accuracy test score of `52%`, and notably, due to the high number of false-positives, produced the lowest low_risk sensitivity score of `43%`.

### SMOTEENN

![alt_text](https://github.com/farwaali08/Credit_Risk_Analysis/blob/040f59338d051adf8a49cf61e5483d0322ba2d24/Images/SMOTEENN.jpg)

   * Balanced accuracy test (appox.): `62%`
   * Precision: `1%`
   * Recall/Sensitivity: `69%`
   * F1: `2%`
   * SMOTEENN, or the combination sampling model ranked in between the SMOTE and ClusterCentroids models, with a balanced accuracy score of about `62%`.

### BalancedRandomForestClassifier

### EasyEnsembleClassifier 
