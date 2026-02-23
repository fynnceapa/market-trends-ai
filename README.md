# Market Trends AI - Prediction Projects

This repository contains data analysis and machine learning models developed to predict prices and demand in two different sectors: the **Automotive Market** (based on Autovit data) and **Bike Sharing Services**.

## Project Overview

The goal of this project is to build end-to-end predictive pipelines, from data cleaning and exploratory analysis to model optimization. We aim to identify key features that influence market trends and provide accurate regression-based forecasts.

## Repository Structure

### 📄 Documentation
* **`raport.pdf`**: A detailed report (in Romanian) describing the methodology, data visualizations, preprocessing steps, and final model performance comparisons for both sub-projects.

### 🚗 Car Price Prediction (Autovit)
* **`autovit.ipynb`**: The primary Jupyter Notebook for the car listing analysis. It includes data cleaning (handling missing values), feature engineering, and training of regression models like Random Forest and Gradient Boosting.
* **`autovit_data/`**:
    * `train_cars_listings.csv`: The primary dataset used for training models.
    * `val_cars_listings.csv`: Dataset used for model validation and testing.

### 🚲 Bike Sharing Demand
* **`bike.ipynb`**: Jupyter Notebook focused on predicting the total number of bike rentals. It analyzes temporal patterns (seasons, holidays) and weather conditions.
* **`bike_data/`**:
    * `train.csv`: Historical data including weather and rental counts for training.
    * `test.csv`: Data used for evaluating model performance.

## Key Features & Methodology
* **Data Preprocessing**: Handled missing values, converted data types (e.g., date-time objects), and performed One-Hot Encoding for categorical features.
* **Exploratory Data Analysis (EDA)**: Includes distribution analysis, correlation matrices, and outlier detection using boxplots.
* **Machine Learning Models**:
    * Linear Regression & SVR
    * Random Forest Regressor
    * Gradient Boosting Regressor (including Quantile Regression for prediction intervals).
* **Evaluation Metrics**: Models were evaluated using Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared ($R^2$) scores through Cross-Validation.

## Requirements
To run the notebooks, you will need:
* Python 3.x
* Pandas, NumPy, Matplotlib, Seaborn
* Scikit-learn