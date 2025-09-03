# Ordinal Classification & Model Optimization - Kaggle ML & DS Survey 2022

## Overview
Built and optimized an ordinal logistic regression model to predict salary ranges based on demographic and technical features, extracted from survey responses.

## Pipeline
### Data Cleaning
- Handles missing values
- encodes categorical features: if ordinal, map to buckets; if nominal, one-hot.

### Exploratory Data Analysis and Feature Selection
- find most relevant features to yearly compensation, via feature importance visualizaiton.
- PCA to reduce dimensionalities.

### Model Implementation
- ordinal logistic regression: train k-1 binary LR classifiers for k class
- 10 fold cv on training
- hyperparam tuning

### Testing 
- evaluate performance (MSE) on test data
- compute bias (expected deviation of pred from true) - variance (how much predictions vary across models trained on different data) tradeoff to see if model overfits/underfits
- visualization of true v.s. prediction
