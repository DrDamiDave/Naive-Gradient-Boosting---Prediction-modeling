# Naive-Gradient-Boosting---Prediction-modeling


The goal is to create an accurate, scalable model that can predict turbidity levels across different locations and times.

## Introduction

Turbidity is a key indicator of water quality and is crucial for monitoring river health. This project leverages machine learning techniques to predict turbidity levels using a combination of remote sensing data and ground-truth measurements.

## Data Sources

Turbidity measurements from three stations.

## Methods

### Data Preprocessing

- **Cleaning and Merging**: Data from different sources were cleaned and merged using a tolerance of one day to ensure alignment.
- **Feature Selection**: Selected relevant features based on Pearson’s correlation and mutual information scores.

### Model Training

- **Algorithms Used**: Naïve Gradient Boosting, Random Forest
- **Training Strategies**:
  - Recent 30% of the data for testing
  - Every fifth measurement for testing
  - Random 30% selection for testing
  - Time-shifted features for potential overfitting

### Hyperparameter Tuning

- **Grid Search**: Employed Grid Search for hyperparameter tuning to optimize model performance.

### Evaluation Metrics

- **R-Squared (R²)**
- **Mean Squared Error (MSE)**

## Results

- **Model Performance**:
  - Best strategy (Strategy 2) achieved a testing R² of 0.3381 and a testing MSE of 863.8.
  - Hyperparameter tuning improved model performance marginally, indicating the need for further optimization.

