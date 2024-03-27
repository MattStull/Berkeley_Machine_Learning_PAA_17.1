# Berkeley_Machine_Learning_PAA_17.1

Jupyter Notebook Link

https://github.com/MattStull/Berkeley_Machine_Learning_PAA_17.1/blob/main/prompt_III.ipynb

Business Understanding

The Business Objective of analyzing the dataset is to develop a predictive model to accurately identify potential clients who are more likely to subscribe to a term deposit offered by the bank. This model aims to enable the bank to target its marketing efforts more effectively, thereby increasing the efficiency of its campaigns and improving the subscription rates for its term deposit products.

Data Understanding and Preparation


1.  As documentation suggested, removed the duration column.
2.  Gender was not included in the data and based on the research paper, gender was equally wighted between classes.
3.  There were no nulls and left unknown labels as unknown.

Modeling

1.  Used SMOTE to proportion labels since 11% of the classes were 1 or accepted a term deposit.
2.  Ran OneHotEncoder on string features and ran StandardScaler() to normalize the data.
3.  The models that were tested were KNN, Decision Tree, Logistic Regression, and Linear SVC (chose this to reduce model run time).

Results

Logistic Regression and Linear SVC had the highest roc_auc scores at 80%.  However, I believe Decision Tree with an accuracy of 85% on trained data and 87% on test data was the best model to use because the precision score was the highest at 42% on the 1 class.  This will ensure the highest efficiency of acceptance for calls made.


