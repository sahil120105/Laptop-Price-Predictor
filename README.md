# Laptop Price Prediction

This project predicts laptop prices based on various specifications such as storage, company, processor, etc. The model uses several machine learning algorithms and techniques to provide accurate price predictions. 

## Features

- **Data Cleaning**: Standard data cleaning techniques to ensure data quality.
- **Exploratory Data Analysis (EDA)**: Identify features that affect the price.
- **Feature Engineering**: Enhance model performance with engineered features.
- **Price Distribution Transformation**: Transform price distribution into a normal distribution for better predictions.
- **Column Transformation**: Use of ColumnTransformer and one-hot encoding with scikit-learn.
- **Pipeline Integration**: Integration of data preprocessing and model training using scikit-learn Pipeline.
- **Model Export**: Exported the trained pipeline for use in Streamlit.

## Algorithms Used

- **Linear Models**: `LinearRegression`, `Ridge`, `Lasso`
- **Neighbors**: `KNeighborsRegressor`
- **Tree-based Models**: `DecisionTreeRegressor`, `RandomForestRegressor`, `GradientBoostingRegressor`, `AdaBoostRegressor`, `ExtraTreesRegressor`
- **Support Vector Machine**: `SVR`
- **XGBoost**: `XGBRegressor`
- **Ensemble Models**: `VotingRegressor`, `StackingRegressor`

## Best Model

The best results were achieved using a `StackingRegressor` with:
- **Base Estimators**: `RandomForestRegressor`, `GradientBoostingRegressor`, `XGBRegressor`
- **Hyperparameter Tuning**: Fine-tuned for optimal performance

## Evaluation Metrics

- **R² Score**: 0.88
- **Mean Absolute Error (MAE)**: 0.16

## Setup and Installation