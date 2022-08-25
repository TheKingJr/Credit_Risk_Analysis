# Credit Risk Analysis Challenge 17

## Overview of Project

The premise of this analysis was to perform credit risk analysis using a series of machine learning algorithms. Primarily using RandonOverSampler, SMOTE, ClusterCentroids, SMOTEENN, BalancedRandomForestClassifier, and EasyEnsembleClassifier. After executing the machine learning models on the credit card dataset from LendingClub, the final step involved evaluating whether or not the performances of these algorithms should be used to predict credit risk. Please see below for the analysis deliverables.

- Deliverable 1: Use Resampling Models to Predict Credit Risk

- Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk

- Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk

- Deliverable 4: A Written Report on the Credit Risk Analysis

## Results

- ### ClusterCentroids
| Balanced Accuracy Score | Precision - High Risk | Precision - Low Risk | Recall - High Risk  | Recall - Low Risk |
|---|---|---|---|---|
| 0.522  |  0.01 |  1.00 | 0.64  | 0.40 |

Brief discussion: The BAS is average, but not good enough for the purposes of predicting credit risk. The precision for both the high and low risk classifications is of high concern. On one spectrum there is very little confidence in the prediction capabilites of this model for high risk lending. On the other spectrum, there is nothing short of overfitting to low risk lending. This is the complete opposite of what we were hoping to achieve regarding this model. Lastly, looking at the recall for both high and low risk classifications, they are decent but not good enough for the purpose we are seeking especially the low risk recall. 

- ### SMOTE
| Balanced Accuracy Score | Precision - High Risk | Precision - Low Risk | Recall - High Risk  | Recall - Low Risk |
|---|---|---|---|---|
| 0.623  |  0.01 |  1.00 | 0.61  | 0.64  |

Brief discussion: The BAS is decent, but not good enough for the purposes of predicting credit risk. The precision for both the high and low risk classifications is of high concern. On one spectrum there is very little confidence in the prediction capabilites of this model for high risk lending. On the other spectrum, there is nothing short of overfitting to low risk lending. This is the complete opposite of what we were hoping to achieve regarding this model. Lastly, looking at the recall for both high and low risk classifications, they are decent but not good enough for the purpose we are seeking. 

- ### RandomOverSampler
| Balanced Accuracy Score | Precision - High Risk | Precision - Low Risk | Recall - High Risk  | Recall - Low Risk |
|---|---|---|---|---|
| 0.646  |  0.01 |  1.00 | 0.61  | 0.68  |

Brief discussion: The BAS is decent, but not good enough for the purposes of predicting credit risk. The precision for both the high and low risk classifications is of high concern. On one spectrum there is very little confidence in the prediction capabilites of this model for high risk lending. On the other spectrum, there is nothing short of overfitting to low risk lending. This is the complete opposite of what we were hoping to achieve regarding this model. Lastly, looking at the recall for both high and low risk classifications, they are decent but not good enough for the purpose we are seeking. 

- ### SMOTEENN
| Balanced Accuracy Score | Precision - High Risk | Precision - Low Risk | Recall - High Risk  | Recall - Low Risk |
|---|---|---|---|---|
| 0.653  |  0.01 |  1.00 | 0.69  | 0.62  |

Brief discussion: The BAS is decent, but not good enough for the purposes of predicting credit risk. The precision for both the high and low risk classifications is of high concern. On one spectrum there is very little confidence in the prediction capabilites of this model for high risk lending. On the other spectrum, there is nothing short of overfitting to low risk lending. This is the complete opposite of what we were hoping to achieve regarding this model. Lastly, looking at the recall for both high and low risk classifications, they are decent but not good enough for the purpose we are seeking. 

- ### BalancedRandomForestClassifier
| Balanced Accuracy Score | Precision - High Risk | Precision - Low Risk | Recall - High Risk  | Recall - Low Risk |
|---|---|---|---|---|
| 0.787  |  0.04 |  1.00 | 0.67  | 0.91  |

Brief discussion: The BAS is the second best in terms of the all the models utilized. Solely regarding the BAS for this model, I'd feel fairly confident in the results it would provide me. However, the precision for both the high and low risk classifications is highly concerning. There is very little precision in predicting high risk candidates for lending and the great likelihood that this model is overfitted to low risk candidate prediction. This is the complete opposite of what we were hoping to achieve regarding this model. Lastly, looking at the recall for both high and low risk classifications. The recall is great for low risk, but only decent for high risk. Thus, this model is good but not good enough for the purpose we are seeking. 

- ### EasyEnsembleClassifier
| Balanced Accuracy Score | Precision - High Risk | Precision - Low Risk | Recall - High Risk  | Recall - Low Risk |
|---|---|---|---|---|
| 0.925  |  0.01 |  1.00 | 0.94  | 0.91  |

Brief discussion: The BAS is the best in terms of the all the models utilized. Solely regarding the BAS for this model, I'd feel very confident in the results it would provide me. However, the precision for both the high and low risk classifications is highly concerning. There is very little precision in predicting high risk candidates for lending and the great likelihood that this model is also overfitted to low risk candidate prediction. This is not what we were hoping to achieve regarding this model. Finally, looking at the recall for both high and low risk classifications. The recall is great for low risk and high risk which is a positive note regarding this algorithm. 

## Summary

Overall, all the algorithms were disappointing to say the least. From a BAS standpoint, they were all decent and above. However, there are major data overfitting issues with the algorithms utilzed. Especially when analyizing the low risk prediction precision for all the models. In regards to the high risk prediction precision, the results were ghastly and the best conclusion to assume would be that there needs to be more data collected in order for these models to perform better. Looking at the recalls for both high and low risk predictions, they were adequate but insufficient for the purposes of this project. The models had a pretty good sensitivity for high risk, but I still wouldn't recommend using any of them. In conclusion, if these algorithms want to be used, a different or larger dataset needs to be provided to better train the models for high risk credit prediction.

