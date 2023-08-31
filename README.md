# ProVision-Time-Series-Ensemble-Models
# Retail Forecasting Models
This Jupyter notebook contains the development and evaluation of 16 gradient boosting machine learning models aimed at forecasting various metrics for a retail company. 

Introduction
[Data Preprocessing]
[Model Descriptions]
[Evaluation Metrics]
[Conclusion]

# Introduction
The retail sector is dynamic, and accurate forecasting is crucial for inventory management, sales strategies, and overall business planning. This notebook aims to provide a comprehensive set of models to predict different aspects of retail performance.

# Data Preprocessing
Before diving into the models, the data undergoes several preprocessing steps:

Handling missing values
Feature engineering, including creating lag features, rolling means, and other time-series specific transformations
Scaling and normalization using techniques like RobustScaler

# Model Descriptions
The notebook explores 16 different models, each tailored for specific forecasting tasks. Here's a brief overview:

Model 1: Daily demand prediction for City 14
Model 2: Daily revenue prediction for City 14

Model 3: Daily demand prediction for City 22
Model 4: Daily revenue prediction for City 22

Model 5: Daily demand prediction for City 31
Model 6: Daily revenue prediction for City 31

Model 7: Daily demand prediction for City 24
Model 8: Daily revenue prediction for City 24

Model 9: Weekly demand prediction for City 14
Model 10: Weekly revenue prediction for City 14

Model 11: Weekly demand prediction for City 22
Model 12: Weekly revenue prediction for City 22

Model 13: Weekly demand prediction for City 31
Model 14: Weekly revenue prediction for City 31

Model 15: Weekly demand prediction for City 24
Model 16: Weekly revenue prediction for City 24

For each model, the following techniques and methodologies are applied:

Pipeline Iteration: The models are first iterated using a pipeline that includes:

 - XGBRegressor
 - LGBMRegressor
 - AdaBoostRegressor
 - CatBoostRegressor

The best-performing model based on preliminary results is then selected for further tuning and evaluation.

Feature Selection: Feature selection is handled by the gradient boosting algorithms since they assign weight to features according to their importances for the model.

Hyperparameter Tuning: Grid Search CV technique is applied to find the optimal set of hyperparameters for each model.

# Evaluation Metrics
Each model is evaluated using a set of metrics to ensure its forecasting accuracy. The primary metrics used are:

 - Root Mean Square Error (RMSE)
 - R-squared (R2)

These metrics provide insights into the model's accuracy and how well it explains the variance in the data.

# Conclusion
This notebook offers a comprehensive set of tools for retail forecasting. By leveraging a combination of traditional and advanced machine learning techniques, it aims to provide accurate and actionable predictions for the retail sector.
These models are used for the development of Pro-Vision App that is placed in a separate repository.
