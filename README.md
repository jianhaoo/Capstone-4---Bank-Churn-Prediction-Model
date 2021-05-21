# Capstone 4 Bank Churn Prediction Model

### Project Summary
The purpose of this project is to create machine learning models to predict the bank customer churn rate. As an data analyst in the bank, i want to identify the factors resulting in customer churns 

###Data Preparation
Performing data cleaning for data. Using Jupyter and Python libraries(Pandas), Several columns such as Customer ID and Customer Name,are indentified as unwanted columns and removed. 

Data Columns After cleaning:
Credit Score
Geography
Age
Gender
Tenure
Balance
Number Of Products
Credit Card 
Active Member
Estimated Salary
Exited

###Initial Insights
Target Variable: Exited
The dataset is imbalanced, having those that has stayed with the bank(Exited==0) totalling around 80%, whereas those that has left(Exited==1) as the remaining 20%.
This issue is being addressed by utilizing SMOTE(Synthetic Minority Over-sampling Technique).

Proportion - Customer Nationality
Around 50% of the customers are from France, around 25% from Spain and also around  25% from Germany. However, we can see a way higher churn coming from Germany, despite having the least customers among the 3 countries.

Customers - Number Of Products
An expected result, which customers that has only 1 product has a higher tendency to churn , where customers with multiple products with the bank have lower churn.

Age and Balance
We can see that customers that are ranged between 40-60 years old, with a higher than average bank balance, are at risk of churning.

###Imbalanced Data - Exited
To fix the issue with imbalanced data, SMOTE was used to create synthetic data from minority class(Exited==1), in order to prepare the data for the machine learning models

###Maching Learning with several models
Logistic Regression
Random Forest
Decision Tree
Neural Network - MLP


###Machine Learning Models Result

Random Forest
Training Accuracy - 0.999294
Testing Accuracy - 0.891086
Precision - 0.891018
Recall - 0.891246
F1 Score - 0.891058

Decision Tree
Training Accuracy - 0.856436
Testing Accuracy - 0.814187
Precision - 0.814112
Recall - 0.813975

F1 Score - 0.891058

![image](https://user-images.githubusercontent.com/34051347/119076834-da107500-ba25-11eb-9832-5e458018cafa.png)



