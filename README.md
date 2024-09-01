Regression of Used Car Prices
This notebook examines various regression models to predict used car prices based on vehicle features and characteristics. The goal is to create a model that can accurately predict prices for cars in the test set to submit predictions for a Kaggle competition.

Data
The training data come from two CSV files located in the Kaggle input directory:

train.csv - contains observations with features and target price variable
test.csv - similar features but missing target prices
Features include vehicle brand, model, year, mileage, fuel type, engine specs, condition ratings and more. The target is the listed price.

Preprocessing
The data are preprocessed to handle missing values, encode categorical features, and split into train/test sets for model evaluation. Features are also standardized for model training.

Modeling
Various regression models are trained on the preprocessed data including:

Random Forest
Gradient Boosting
Decision Tree
KNN
XGBoost
CatBoost
Voting ensemble
Models are evaluated on the test set using RMSE, MAE and R^2.

Predictions
The best performing CatBoost model is used to make predictions on the test data. A submission CSV file is created with id and predicted price columns for uploading to Kaggle.

Summary
This notebook explores regression techniques for predicting used vehicle prices. The ensemble CatBoost model performs well and its predictions are submitted for evaluation on hidden test data. Further tuning may help improve results.
