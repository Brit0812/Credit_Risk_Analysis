# Credit_Risk_Analysis

# Overview

The purpose of providing this analysis is to provide predictions, based on the data, using supervised machine learning. The goal was to provide a credit risk assessment: are they a good applicant? Are they trust worthy? What are the factors that make someone a high-risk credit applicant? 

In order to proceed with using machine learning, the data needs to “fit” the models being used. Shaping the data into usable data, that would be easily read and fed into the machine learning model. An issue with the data set provided was there were a lot of acceptable credit applicants vs the high-risk applicants. When one outweighs the other the model will more than likely incorrectly categorize future applicants. Since the model is likely to see someone who should be approved it will likely approve them as it doesn’t see many high-risk credit applicants. Especially when it comes to outliers or those who are on the line of being approved or denied. In order to correct the skewed data multiple imports are used to the correct the imbalanced data. 

# Results

The balanced accuracy score, the precision and the recall scores of the 6 machine learning models, is as follows: 

## Naïve Random Oversampling

![](images/oversample_acc.png)

•	balanced accuracy: 0.6456 

o	64.6% accuracy 

![](images/oversample_report.png)

•	Precision: 

o	low-risk precision: 0.01

o	high-risk precision: 1.00

•	Recall: 

o	High-risk: 0.61

o	Low-risk: 0.68

## SMOTE Oversampling 

Image- balanced accuracy-SMOTE
•	balanced accuracy: 0.6234
o	62.3% accuracy 
Image- classification report-SMOTE
•	Precision: 
o	low-risk precision: 0.01
o	high-risk precision: 1.00
•	Recall: 
o	High-risk: 0.61
o	Low-risk: 0.64

## Undersampling 

Image- balanced accuracy-under
•	balanced accuracy: 0.5102
o	51% accuracy 
Image- classification report-under
•	Precision: 
o	low-risk precision: 0.01
o	high-risk precision: 1.00
•	Recall: 
o	High-risk: 0.57
o	Low-risk: 0.45

## Combination (Over and Under) Sampling

Image- balanced accuracy- combo
•	balanced accuracy: 0.6396 
o	64% accuracy 
Image- classification report-combo
•	Precision: 
o	low-risk precision: 0.01
o	high-risk precision: 1.00
•	Recall: 
o	High-risk: 0.70
o	Low-risk: 0.58


## Balanced Random Forest Classifier

Image- balanced accuracy-BRFC
•	balanced accuracy: 0.7886
o	79% accuracy-BRFC
Image- classification report
•	Precision: 
o	low-risk precision: 0.03
o	high-risk precision: 1.00
•	Recall: 
o	High-risk: 0.70
o	Low-risk: 0.87


## Easy Ensemble AdaBoost Classifier

Image- balanced accuracy-EEABC
•	balanced accuracy: 0.9317
o	93.2% accuracy 
Image- classification report-EEABC
•	Precision: 
o	low-risk precision: 0.09
o	high-risk precision: 1.00
•	Recall: 
o	High-risk: 0.92
o	Low-risk: 0.94


# Summary 
After performing six machine learning models, only two models had an accuracy that was more than 70%. But, of the two, one proved to be incredibly efficient as its accuracy was 93.2%! The best machine learning model is the Easy Ensemble AdaBoost Classifier. When looking at the precision of each of the models, they all look fairly similar as the low-risk candidates stand between 0.1 and 0.9 while high-risk candidates stand at 1.0. It’s important to note the recall of each model as well, as its value will stand between 0 and 1 like the accuracy. The higher the recall value the better the model: proving the best model for our purpose would be the Easy Ensemble AdaBoost Classifier model.

