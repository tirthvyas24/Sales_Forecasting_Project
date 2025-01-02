# Sales_Forecasting_Project
## Overview
This project involves building a machine learning model to predict sales for retail items based on historical data. The dataset contains various features such as item details, store information, and historical sales data. The project focuses on data preprocessing, feature engineering, and model evaluation.

## Key Features
- **Data Preprocessing**: 
  - Handled missing values and outliers.
  - Encoded categorical variables using Label Encoding and One-Hot Encoding.
  - Applied log transformation to reduce skewness and outliers.

- **Feature Engineering**:
  - Created new features like the number of years a store has been operational.
  - Consolidated similar categories for uniformity.

- **Modeling**:
  - Implemented Random Forest Regression.
  - Fine-tuned hyperparameters using RandomizedSearchCV.
  - Evaluated the model using R² Score, Mean Absolute Error (MAE), and Mean Squared Error (MSE).

## Tools and Libraries
- **Programming Language**: Python
- **Libraries**:
  - Data Manipulation: Pandas, Numpy
  - Visualization: Matplotlib, Seaborn
  - Machine Learning: Scikit-learn

## Dataset
The dataset contains information about:
- Item details (e.g., weight, visibility, type, and price).
- Outlet information (e.g., type, size, location, and establishment year).
- Target variable: Sales for each item at different outlets.

## Steps Performed
1. **Data Cleaning**:
   - Replaced missing values in `Item_Weight` and `Outlet_Size` using group means and modes.
   - Replaced zeros in `Item_Visibility` with the mean.

2. **Exploratory Data Analysis (EDA)**:
   - Analyzed data distributions with histograms and count plots.
   - Correlation analysis using heatmaps.

3. **Feature Engineering**:
   - Created `New_Item_Type` based on the first two characters of `Item_Identifier`.
   - Added `Outlet_Years` to capture the store’s operational years.

4. **Modeling**:
   - Trained a Random Forest Regressor.
   - Optimized hyperparameters using RandomizedSearchCV.
   - Evaluated the model’s performance.

5. **Results**:
   - Achieved good accuracy in predicting sales.
   - Gained insights into feature importance.
