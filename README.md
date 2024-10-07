﻿# CodSoft
# IMDB Movie Rating Prediction
Project Overview
This project is part of my Data Science Internship at CodSoft. It focuses on predicting movie ratings from the IMDB Movies India dataset using a variety of regression models. The goal was to use various features such as actors, director, duration, and user votes to accurately predict a movie's rating.

**Dataset**
The dataset includes information on:

Movie name
Director and actors
Genre
Duration and year of release
User votes and ratings
Project Workflow

**1. Data Cleaning and Preprocessing**
Handling Missing Values:
Missing data in categorical columns (e.g., director, actor) was replaced with placeholders such as Unknown Director or Unknown Actor.
KNN Imputer was used to handle missing values in numeric columns like Votes, Duration, and Rating.
Text Processing:

Extracted the year from the 'Year' column and cleaned the 'Name' column.
Converted the 'Votes' column to numerical values, handling shorthand notation (e.g., 'K' for thousands, 'M' for millions).
Genre Encoding:

NaN values in the 'Genre' column were replaced with Unknown Genre.
One-hot encoding was applied to handle multiple genres for each movie.
**2. Feature Engineering**
Target Encoding:
Used means encoding for categorical features such as Director, Actor 1, Actor 2, and Actor 3.

**3. Model Building and Evaluation**
We applied four different regression models to predict the movie ratings:

Lasso Regression: Utilized for feature selection and regularization.
Random Forest Regressor: Applied for its ensemble learning capabilities, achieving high accuracy with a 95.7% R² score.
Gradient Boosting Regressor: Further boosted performance with an adaptive learning approach.
AdaBoost Regressor: Implemented for additional boosting.

**4. Model Evaluation Metrics:**
Mean Squared Error (MSE) and Root Mean Squared Error (RMSE) were used to evaluate model performance.
R² score was calculated for each model to assess how well the models explained the variability in the data.

**5. Results**
Random Forest Regressor gave the best performance with:
Mean Squared Error (MSE): 0.083
Root Mean Squared Error (RMSE): 0.288
R² score: 0.957

**Conclusion**
This project demonstrated the power of ensemble methods like Random Forest and Gradient Boosting in regression tasks. It also highlights the importance of thorough data cleaning, feature engineering, and model tuning for accurate predictions.
