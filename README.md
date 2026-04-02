Lab 6: Linear Regression – Ecommerce Customers
Course: ARTI308 - Machine Learning

Overview
This lab applies Linear Regression to predict how much a customer will spend yearly on an e-commerce platform. The work follows the same workflow introduced in the lab tutorial (USA Housing dataset) and applies it end-to-end on a new dataset.

Dataset
File: Ecommerce_Customers.csv
Rows: 500 | Columns: 8
ColumnTypeDescriptionEmailTextCustomer email (not used in model)AddressTextCustomer address (not used in model)AvatarTextAvatar color/name (not used in model)Avg. Session LengthFloatAverage session duration on the platformTime on AppFloatAverage time spent on the mobile app (minutes)Time on WebsiteFloatAverage time spent on the website (minutes)Length of MembershipFloatNumber of years the customer has been a memberYearly Amount SpentFloatTarget variable — total spending per year ($)

Steps Performed

Import Libraries : pandas, numpy, matplotlib, seaborn, scikit-learn
Load Data : Read CSV into a DataFrame
Explore Data : .head(), .info(), .describe(), missing value check
EDA : Pairplot, target distribution histogram, correlation heatmap
Feature Engineering : Dropped non-numeric columns; used the 4 numerical features
Train-Test Split : 60% train / 40% test, random_state=101
Train Model : sklearn.linear_model.LinearRegression
Evaluate : Actual vs. Predicted scatter plot, residuals histogram, error metrics
