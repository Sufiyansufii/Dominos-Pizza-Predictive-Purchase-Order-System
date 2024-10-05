# Domino's Pizza - Predictive Purchase Order System
# Project Overview
This project aims to develop a predictive purchase order system for Domino's Pizza by analyzing historical sales and ingredient data. The goal is to forecast future pizza sales, optimize inventory management, and minimize waste while ensuring ingredient availability.

# Skills Acquired
Data cleaning and preprocessing
Exploratory Data Analysis (EDA)
Time series forecasting
Predictive modeling
Business decision making
Real-world application of data science
# Domain
Food Service Industry

# Problem Statement
Domino's Pizza aims to optimize the ordering process for ingredients by accurately predicting future sales. This project leverages historical sales data and ingredient information to create a predictive model that generates efficient purchase orders, thereby minimizing waste and preventing stockouts.

# Business Use Cases
# Inventory Management: 
Maintain optimal stock levels to meet future demand without overstocking.
# Cost Reduction: 
Minimize waste and reduce costs associated with expired or excess inventory.
# Sales Forecasting: 
Accurately predict sales trends to inform business strategies and promotions.
# Supply Chain Optimization: 
Streamline the ordering process to align with predicted sales and avoid disruptions.
# Dataset Information
# Sales Dataset: 
Contains historical sales records, including Date, Pizza Type, Quantity Sold, Price, Category, and Ingredients.
# Ingredients Dataset: 
Contains ingredient requirements for each pizza type, detailing Pizza Type, Ingredient, and Quantity Needed.
# Prerequisites
Ensure you have the following Python libraries installed:

pandas
numpy
matplotlib
seaborn
openpyxl (for reading Excel files)
sklearn
statsmodels
tensorflow
You can install the necessary dependencies using:

# Steps Performed
# 1. Data Loading
The project begins by loading the sales and ingredients datasets from Excel files.

# 2. Data Cleaning and Preprocessing
# Converting Data Types: 
The order_date and order_time columns were converted to appropriate datetime formats.
# Identifying and Handling Missing Values: 
Critical columns such as pizza_name, pizza_category, and total_price were checked for missing values and filled accordingly.
# Outlier Removal: 
Outliers in the quantity column were identified and handled using the Interquartile Range (IQR) method.
# 3. Feature Engineering
Various date-related features were extracted, including day_of_week, day_of_year, week_of_year, and month, which aid in predicting sales trends.

# 4. Exploratory Data Analysis (EDA)
Sales trends over time were visualized, along with quantities sold by category and top-selling pizzas.
Ingredient usage per pizza was analyzed to understand ingredient demands better.
# 5. Time Series Analysis
The sales data for selected pizzas was plotted to observe sales trends, seasonality, and patterns over time.

# 6. Predictive Modeling
Data was split into training and testing sets.
Various regression models were built, including Linear Regression, ARIMA, SARIMA, Decision Tree Regressor, Random Forest Regressor, and Gradient Boosting Regressor.
Model performance metrics (MAPE, MSE, MAE, R², RMSE) were calculated for each model.
# 7. Saving Cleaned Data
The cleaned sales and ingredients datasets were saved to new Excel files for future use in modeling.

# Future Steps
The next phase of the project will involve:

Building the predictive model using the cleaned datasets.
Implementing hyperparameter tuning for models to improve performance.
Generating detailed purchase orders based on the predicted sales.
# Conclusion
This project involves a comprehensive cleaning and preprocessing phase for the Domino's Pizza sales and ingredients datasets. The missing values were addressed, data points were corrected, and the datasets were prepared for model building. Future work will focus on model training, evaluation, and integration of a purchase order generation system.
