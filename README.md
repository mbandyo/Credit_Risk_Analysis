# Credit Risk Analysis
This project builds and compares several models using different methodologies for supervised Machine Learning and compares model performances.
Predicting credit risk is an imprtant aspect for lenders. The accuracy of credit risk predition would enable a lender avoid approving risky loans and charging appropriate risk premiums. However, a strict and conservative lending policy would hurt the business, market share, revenues and profits and reputation of the institution. This could threaten the sustainability of the business. Therefore, it is very important for a lending institution to assess the risk of a loan and balance this risk with ongoing business sustainability. 
The challenge of using standard methods are that sometimes the decisions need to be made fairly quickly with limited data. Since the number of defaults are small compared to the number of loans issued, traditional statistical methods may be challening in adeqaute loan risk assessment. The industry is increasingly using ML languages for these type of modeling for robust analysis. Also credit is a highly regulated industry and the business practices are scrutinized by regulators in great detail and punitive actions are imposed on the lending institutions for smallest violations.  Therefore, it is important for a lending instutions to robust models to manage both business and regulatory risks.
## Models and Performances
#### Oversampling Results
The model outcome is the dependent variable loan status as high risk/low risk.
* Naive Random Oversampling: </br>
Following are the perrformance metrics:
Naive Random Oversampling results: Our balanced accuracy test is 64%, the precision for the high_risk has a very low positivity at 1% and the recall is 69%
Interpretation: Due to low precision of high_risk prediction, this model is not very good for high_risk assessment. Also a low (2%) F1 score indicates the model flags high number of false positives and false negatives.
![image](https://user-images.githubusercontent.com/31217096/201537714-c48bf055-b367-4488-81ef-552bedfca34a.png)

* SMOTE Oversampling:</br>
The following are model performance metrics:
Balanced accuracy test: 66%   ; precision for high_risk positivity: 1% recall: 63%
Interpretation: Due to low precision of high_risk prediction, this model is not very good for high_risk assessment. 
Also a low (2%) F1 score indicates the model flags high number of false positives and false negatives.
![image](https://user-images.githubusercontent.com/31217096/201538248-364fa098-dd1d-4fa1-b653-ca274ca8bf6c.png)
#### Undersampling Results:
* Clustercentroid Resampler:
 Balanced accuracy test: 66%  ; precision for high_risk positivity: 1% recall: 69%. 
Interpretation: Due to low precision of high_risk prediction, this model is not very good for high_risk assessment. 
Also a low (2%) F1 score indicates the model flags high number of false positives and false negatives.
![image](https://user-images.githubusercontent.com/31217096/201540861-e3e63336-e033-40a3-a378-b9b49d0b8984.png)


#### Combination (Over and Under) Sampling:
* SMOTEEN Sampling:
Balanced accuracy test: 54%  ; precision for high_risk positivity: 1% recall: 72%
Interpretation: Due to low precision of high_risk prediction, this model is not very good for high_risk assessment. 
Also a low (2%) F1 score indicates the model flags high number of false positives and false negatives.
![image](https://user-images.githubusercontent.com/31217096/201542118-05960d58-e0ef-4524-ac9f-8f64a8e554cf.png)

#### Ensemble Learners:
* Balanced Random Forest Classifier:
 Balanced accuracy test: 76%  ; precision for high_risk positivity: 3% recall: 64%
Interpretation: Due to low precision of high_risk prediction, this model is not very good for high_risk assessment. 
Also a low (6%) F1 score indicates the model flags high number of false positives and false negatives.
![image](https://user-images.githubusercontent.com/31217096/201542310-1c6c99a9-7f1b-410a-93b2-a3762351a3df.png)

* Easy Ensemble AdaBoost Classifier:
Balanced accuracy test: 91%  ; precision for high_risk positivity: 9% recall: 89%
Interpretation: Due to low precision of high_risk prediction, this model is not very good for high_risk assessment. 
Also a low (16%) F1 score indicates the model flags relatively high number of false positives and false negatives.
![image](https://user-images.githubusercontent.com/31217096/201542492-c2af7684-b4d6-42f3-9e64-1cc584aef8b6.png)

### Summary
The performance of the models considered for credit risk prediction are not very good. However, some of it may be a result of a relatively small dataset. 
### Recommendation
Of all the models considered so far, the Easy Ensemble Adaboost classifier has recorded best performance. Although a better precision and F1 score are desirable, this is the best performing model among the available choices.











