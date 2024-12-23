# Rotten Tomatoes Dataset Analysis
This repository contains a comprehensive analysis of the Rotten Tomatoes dataset, focusing on predicting audience ratings using various machine learning techniques.

## Project Overview
The goal of this project was to predict audience ratings using machine learning models, evaluating their performance on all features versus selected features. After exploring and training multiple models, **XGBoost** emerged as the best-performing model, achieving the highest R² score and lowest RMSE.

## Features and Approach

1. **Dataset Cleaning:**  
   - Preprocessed the dataset to handle missing values, remove duplicates, and normalize data.

2. **Feature Selection:**  
   - Compared predictions using all features against a subset of selected features to assess model performance.

3. **Machine Learning Models Used:**  
   - **Support Vector Regression (SVR)**  
   - **Random Forest Regressor**  
   - **XGBoost Regressor**

4. **Hyperparameter Tuning:**  
   - Employed GridSearchCV with 5-fold cross-validation to fine-tune model parameters.

## Key Results

### Best Model: XGBoost
- **Best Hyperparameters:**  
  - `colsample_bytree`: 0.8  
  - `learning_rate`: 0.1  
  - `max_depth`: 7  
  - `n_estimators`: 200  
  - `subsample`: 0.8  

### Performance Metrics
- **Root Mean Squared Error (RMSE):** 14.07  
- **R² Score:** 0.51  

These results indicate that XGBoost provided a good balance between model complexity and performance, explaining around 51% of the variance in audience ratings.

### Prediction Example
After training the XGBoost model, a prediction function was created to predict audience ratings based on movie details.

- **Predicted Audience Rating:** 66.17  
- **Actual Rating (from dataset):** 66  

## Key Insights
- Models trained with all features consistently outperformed those trained on selected features.
- XGBoost was the most effective model, with robust hyperparameter tuning enhancing its performance.

## Future Work
- Explore additional features and external datasets to improve prediction accuracy.
- Investigate deep learning techniques for enhanced model performance.
