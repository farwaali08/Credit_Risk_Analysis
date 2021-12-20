# Credit_Risk_Analysis

## OVERVIEW

For this project, Python was used to create and assess several machine learning models in order to predict credit risk. The data was obtained from LendingClub, a lending-services company, and contains over `68,000` usable entries. Data pertaining to credit risk is notoriously unbalanced, as good loans generally outnumber risky ones, and it was no different in this instance:

The data was resampled using the different methods outlined below, and then each method was evaluated based on its performance.



| **Oversampling** | **Undersampling**|**Both**         |**Ensemble Methods**          |
|----------------- | -----------------|-----------------|-----------------             |
| RandomOverSampler| ClusterCentroids |SMOTEEN          |BalancedRandomForestClassifier|               
| SMOTE            |                  |                 |EasyEnsembleClassifier        |


**Note**: the ensemble methods are machine learning models that reduce bias by generating under-sampled subsets combined inside an ensemble. **EasyEnsembleClassifier** is a boosting algorithm, and **BalancedRandomForestClassifier** is a bagging algorithm.

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

### SMOTE

### ClusterCentroids

### SMOTEENN

### BalancedRandomForestClassifier

### EasyEnsembleClassifier 
