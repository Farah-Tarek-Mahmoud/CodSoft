# Advertising Sales Prediction

This project aims to predict sales based on advertising spending across three channels: TV, Radio, and Newspaper. Two regression models are implemented for comparison: **Random Forest Regressor** and **OLS Linear Regression**.

## Dataset
The dataset contains advertising spend on:
- **TV**: Advertising spend on TV.
- **Radio**: Advertising spend on Radio.
- **Newspaper**: Advertising spend on Newspapers.
- **Sales**: The target variable, representing the sales generated.

### Columns:
- **TV**: TV advertising budget.
- **Radio**: Radio advertising budget.
- **Newspaper**: Newspaper advertising budget.
- **Sales**: Sales outcome (target variable).

## Project Steps:
1. **Exploratory Data Analysis (EDA)**:
   - Summary statistics and data visualization.
   - Correlation analysis.
   - Distribution of features and target variable.

2. **Data Preprocessing**:
   - Check for missing values.
   - Splitting data into training and testing sets (80/20 split).

3. **Modeling**:
   - **Random Forest Regressor**:
     - Initial training and evaluation.
     - Cross-validation and hyperparameter tuning using `RandomizedSearchCV`.
   - **OLS Linear Regression**:
     - Model fitting using `statsmodels`.
     - Evaluation of regression coefficients, residuals, and model summary.

4. **Model Evaluation**:
   - **Metrics Used**:
     - Mean Absolute Error (MAE)
     - Mean Squared Error (MSE)
     - R-squared (R²)
     - Root Mean Squared Error (RMSE)
   - Comparison of models based on performance metrics.

## Key Results:
- **Random Forest Regressor**: After tuning, the model was optimized with hyperparameters such as number of estimators, maximum depth, and minimum samples for splits.
- **OLS Linear Regression**: Provided insights into feature significance and fit using traditional regression metrics.

## Installation:
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/advertising-sales-prediction.git
