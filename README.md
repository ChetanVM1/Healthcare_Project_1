# Diagnosis of impacting factors on hospital readmission rate

 Binary classification problem

Centres for Medicare Services in USA established the Hospital Readmissions Reduction Program. The aim of the program was to improve the healthcare facilities provided hospitals in USA and therefore, reduce the medical expenses of patients. It is achieved by penalising those hospitals which are having more hospital readmission rates than expected.

The objective of the project was to diagnose the impacting factors that cause readmission of patients. If a patient is discharged from a hospital and due to some reasons, the patient is readmitted again within the 30 days of discharge, then it is considered as readmission of patient for the presented analysis.

The data was taken from WHO website. It has more than 1 lack rows of patient records on rows with 50 columns. 

Data cleaning operations are performed. There were some major challenges that we faced during the project. For example, there were null entries in dataset. We tackled it by various imputing method. The data was imbalanced. SMOTE technique was used to treat imbalance in dataset. By determining IQR, outliers from the dataset were removed.

Feature engineering, exploratory data analysis, feature scaling, feature transformation was performed before train test split. Since it was binary classification problem, we selected logistic regression as base model. Assumptions of logistic regression model were verified.

After removing the multicollinearity, we tried different classification models such as decision tree, random forest, different ensemble techniques such as adaboost, gradient boost, xgboost. Random forest model with top 10 significant features were showing the best accuracy results on test dataset (i.e., 94%). So, the same model was hyper-tuned further which increased the accuracy by 1%
