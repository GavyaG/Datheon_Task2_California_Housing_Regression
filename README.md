# Task 2: California Housing Price Prediction

## Project Overview

This project focuses on predicting California housing prices using machine learning regression algorithms. The California Housing dataset is used to explore relationships between housing features and median house values.

The project includes data preprocessing, exploratory data analysis, feature engineering, multicollinearity analysis, model training, hyperparameter tuning, and performance evaluation.

## Objective

To build and compare regression models that predict median house values and identify the best-performing model.

## Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Statsmodels

## Dataset

**Dataset:** California Housing Dataset

- Total Records: 20,640
- Original Features: 8 input features
- Target Variable: `median_house_value`

## Project Workflow

### 1. Data Loading
- Imported the required libraries.
- Loaded the California Housing dataset.
- Examined dataset structure and statistical information.

### 2. Exploratory Data Analysis
- Analyzed numerical features.
- Visualized feature distributions.
- Created correlation heatmaps.

### 3. Data Preprocessing
- Identified missing values.
- Handled missing values using median imputation.
- Applied StandardScaler to numerical features.
- Applied OneHotEncoder to categorical features.

### 4. Feature Engineering
- Created `rooms_per_household`.
- Created `bedrooms_per_room`.
- Created `population_per_household`.
- Created an interaction feature using median income and housing median age.

### 5. Multicollinearity Analysis
- Calculated Variance Inflation Factor (VIF).
- Identified highly correlated features.
- Removed features with high VIF values.
- Recalculated VIF to evaluate the updated features.

### 6. Model Training
Implemented three regression algorithms:

- Ordinary Least Squares (OLS) Regression
- Ridge Regression
- Lasso Regression

### 7. Hyperparameter Tuning
- Used GridSearchCV.
- Tuned Ridge and Lasso regularization parameters.
- Applied 5-fold cross-validation.

### 8. Model Evaluation

Evaluated model performance using:

- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- R² Score

### 9. Visualization
- RMSE comparison chart.
- Actual vs. Predicted plots.
- Residual distribution analysis.

## Final Model Performance

| Model | RMSE | MAE | R² Score |
|---|---:|---:|---:|
| OLS | 76414.2677 | 52720.7071 | 0.5544 |
| Ridge | 76422.3339 | 52727.4811 | 0.5543 |
| Lasso | 76414.6372 | 52721.6498 | 0.5544 |

## Best Performing Model

**OLS Regression**

OLS achieved the lowest RMSE and MAE among the three evaluated models.

## Key Learnings

- Exploratory Data Analysis
- Handling missing values
- Feature Engineering
- Multicollinearity Analysis using VIF
- Regression Algorithms
- Regularization Techniques
- Hyperparameter Tuning
- Model Evaluation and Visualization

## Project Files

```text
Task 2/
│
├── housing.csv
├── Datheon_Task2_California_Housing_Regression.ipynb
└── README.md
```

## Internship

**Organization:** Datheon  
**Program:** Machine Learning & Data Science Internship  
**Task:** Task 2 – California Housing Price Prediction
