# LoanDefaultPrediction

INTRODUCTION
In financial institutions, loans are not given to just anyone who applies for it; a credit risk analysis is used to determine whether a person qualifies for a loan or not. Credit risk assessment is the means of assessing the probability that a customer will default on a loan payment. Using basic classification techniques (Logistic Regression, SVM, Decision trees, KNN), I built and improved models that can help assess customer's ability to repay a loan. 

The dataset, gotten from Kaggle, contains 10000 customers, three features (Employment status, Bank Balance and Annual Salary) of each customer and a Marker that denotes whether or not they defaulted on loan repayment.


EDA and Data Profiling
The dataset was clean and had no null values. However, it was largely imbalanced with only 333 customers of 10000 being loan defaulters. An imbalance in data means that the model will perform much better in predicting the majority class (non-defaulters) than the minority class (defaulters). Later in the project, resampling techniques were used to reduce the effect of imbalance on the models.

Visualizations and descriptive analysis revealed some insights about both classes of customers according to the dataset. It was observed that the defaulters all earned more than $115000 annually and had a bank balance of more than $7800 at the time of loan application.

MODELLING
The data was then split into a training set to help train the models and a test set to help evaluate the models' performance. Of all the basic classification techniques with some hyperparameter tuning, the Logistic regression model performed best and was later improved upon using random resampling on the minority class. 

MODEL PERFORMANCE AND CONCLUSION
The final model achieved an impressive accuracy score of 98% and will precisely spot a defaulter 63% of the time using only three features- Employment status, Bank Balance and Annual salary. 
For excellent credit risk analysis, more features such as age group, number of children and even marital status will be required to improve the performance of the model at spotting defaulters. Also, better models such and Random Forest, Xgboost, e.t.c, may achieve better classification scores, but the aim of this project was to exercise my skills on the basic supervised classification modelling techniques.
