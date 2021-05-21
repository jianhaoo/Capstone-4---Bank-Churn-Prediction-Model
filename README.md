# Capstone 4 Bank Churn Prediction Model

### Project Summary
The purpose of this project is to create machine learning models to predict the bank customer churn rate. As an data analyst in the bank, i want to identify the factors resulting in customer churns 

###Data Preparation
Performing data cleaning for data. Using Jupyter and Python libraries(Pandas), Several columns such as Customer ID and Customer Name,are indentified as unwanted columns and removed. 

Data Columns After cleaning:
![image](https://user-images.githubusercontent.com/34051347/119076890-ef859f00-ba25-11eb-93d5-1c640116ec38.png)

###Initial Insights
Target Variable: Exited
The dataset is imbalanced, having those that has stayed with the bank(Exited==0) totalling around 80%, whereas those that has left(Exited==1) as the remaining 20%.
This issue is being addressed by utilizing SMOTE(Synthetic Minority Over-sampling Technique).
![image](https://user-images.githubusercontent.com/34051347/119076944-07f5b980-ba26-11eb-8653-08a60170c163.png)
![image](https://user-images.githubusercontent.com/34051347/119076990-17750280-ba26-11eb-8182-128f0f2d31e3.png)

Proportion - Customer Nationality
Around 50% of the customers are from France, around 25% from Spain and also around  25% from Germany. However, we can see a way higher churn coming from Germany, despite having the least customers among the 3 countries.

![image](https://user-images.githubusercontent.com/34051347/119076961-0deb9a80-ba26-11eb-8f99-e328b6947991.png)


Customers - Number Of Products
An expected result, which customers that has only 1 product has a higher tendency to churn , where customers with multiple products with the bank have lower churn.
![image](https://user-images.githubusercontent.com/34051347/119077014-2065d400-ba26-11eb-800f-7beb9ad96e4c.png)

Age and Balance
We can see that customers that are ranged between 40-60 years old, with a higher than average bank balance, are at risk of churning.
![image](https://user-images.githubusercontent.com/34051347/119077029-28257880-ba26-11eb-8e85-135973865e86.png)


###Imbalanced Data - Exited
To fix the issue with imbalanced data, SMOTE was used to create synthetic data from minority class(Exited==1), in order to prepare the data for the machine learning models

###Maching Learning with several models
Logistic Regression
Random Forest
Decision Tree
Neural Network - MLP


###Machine Learning Models Result

![image](https://user-images.githubusercontent.com/34051347/119076834-da107500-ba25-11eb-9832-5e458018cafa.png)


###Feature Importance
We have identified that Age,Number Of Products and Balance are the top 3.
![image](https://user-images.githubusercontent.com/34051347/119077060-34113a80-ba26-11eb-89cf-c87a4508b0b9.png)




