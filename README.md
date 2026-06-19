# 🏡 California Housing Price Predictor: End-to-End ML Pipeline

## 📖 Overview
This repository contains a complete, production-style Machine Learning pipeline designed to predict median house values in California based on district metrics (population, median income, location, etc.). 

The project demonstrates a structured approach to a regression problem, moving from raw data exploration to a fully tuned ensemble model, utilizing best practices like Scikit-Learn `Pipeline` and `ColumnTransformer` to prevent data leakage and ensure reproducibility.

## ✨ Features
* **Exploratory Data Analysis (EDA):** Visualizations of feature distributions, missing value analysis, and correlation heatmaps using Seaborn and Matplotlib.
* **Robust Preprocessing:** Automated handling of missing values (median/most frequent imputation), standard scaling for numerical features, and one-hot encoding for categorical variables.
* **Model Evaluation (Cross-Validation):** Evaluated multiple algorithms using 5-Fold Cross-Validation:
  * Linear Regression (Baseline)
  * Ridge & Lasso Regression
  * Random Forest Regressor
  * Histogram-based Gradient Boosting (HistGradientBoostingRegressor)
* **Hyperparameter Tuning:** Utilized `GridSearchCV` to optimize learning rates, tree depth, and L2 regularization for the top-performing model.
* **Inference Pipeline:** A ready-to-use Python function that accepts raw new data and passes it through the preprocessing and modeling steps to output a final price prediction.

## 🛠️ Technologies & Libraries Used
* **Python 3.12.4
* **Pandas & NumPy:** Data manipulation and numerical operations.
* **Scikit-Learn:** Machine learning models, pipelines, metrics, and cross-validation.
* **Matplotlib & Seaborn:** Data visualization.