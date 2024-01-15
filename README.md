# Telco Customer Churn - Predicting Behavior to Retain Customers

The primary goal of this project is to investigate and understand the factors that influence customer churn in the telecom industry, as well as to develop strategies for customer retention. The project's goal is to identify patterns and trends in customer behavior and then use that knowledge to design and implement targeted retention programs. The ultimate goal is to assist the telecom company in developing an effective retention strategy based on the results of our model, which will help the company keep their customers satisfied and engaged.

DATA WRANGLING:

The Kaggle data on Telco Customer Churn was obtained from the IBM analytics community. The dataset has 7043 rows and 21 features, with 17 categorical and 3 numerical variables. Customer demographics, services subscribed to by the customer, and account information are among the variables. The classification ratio for the target variable 'Churn' is 73%-27%. (No -Yes)

To ensure data quality and consistency, data preprocessing was performed. The steps were as follows:
- The 'TotalCharges' column was converted from an object to a numeric type.
- 22 duplicate rows were identified and removed to ensure that each customer was represented only once.
- 11 missing values were checked and removed.
- Outlier detection yielded no results.
- Dummy variables for categorical variables are created to allow for further analysis.

EXPLORATORY DATA ANALYSIS
According to the EDA, churn within the gender distribution was roughly equal, with no significant difference in the number of males and females. Customers with month-to-month contracts churned at a higher rate than those with one- or two-year contracts. Customers who churned their phone service were likely to be non-seniors, without partners, and without dependents. According to the correlation matrix, month-to-month contracts have the highest correlation with customer churn.

![alt text](https://github.com/gabrieljonathan164/Customer_Churn/blob/main/Images/EDA1.jpg)    ![alt text](https://github.com/gabrieljonathan164/Customer_Churn/blob/main/Images/EDA2.jpg)

![alt text](https://github.com/gabrieljonathan164/Customer_Churn/blob/main/Images/EDA3.jpg)    ![alt text](https://github.com/gabrieljonathan164/Customer_Churn/blob/main/Images/EDA4.jpg)

![alt text](https://github.com/gabrieljonathan164/Customer_Churn/blob/main/Images/EDA5.jpg)


MACHINE LEARNING MODELS:
Logistic Regression, Decision Trees, and Random Forests were among the supervised machine learning models used in the project. SelectKBest was used to select top features with a high impact on the Churn variable, SMOTE Oversampling to balance the data and resample, and GridSearchCV for hyperparameter tuning.

RESULTS AND ANALYSIS
The accuracy and F1-score of the models were used to assess their performance. The Random Forest model was 88% accurate and had an F1-score of 90%. 

![alt text](https://github.com/gabrieljonathan164/Customer_Churn/blob/main/Images/EDA6.jpg)
