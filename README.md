# House Price Prediction using Advanced Regression

## Project Overview
This project aims to predict house prices using a dataset from a Kaggle competition. I followed a full data science workflow, including data cleaning, exploratory data analysis (EDA), and the implementation of multiple regression models. The final analysis provides a reliable tool for predicting house values and demonstrates a professional approach to solving a real-world problem.

## Methodology
1.  **Data Preprocessing:** I handled missing values, removed outliers, and applied a log transformation to the `SalePrice` variable to normalize its distribution.
2.  **Exploratory Data Analysis (EDA):** I explored key features, their distributions, and correlations with the target variable. A correlation heatmap revealed that `OverallQual` and `GrLivArea` were the most correlated features with `SalePrice`. A statistical T-test confirmed that houses with higher `OverallQual` have a statistically significant higher sale price.
3.  **Model Building:** I built and evaluated four different regression models: Linear Regression (as a baseline), Lasso Regression, XGBoost, and Random Forest Regressor.

## Model Performance
I evaluated each model using Root Mean Squared Error (RMSE), R² score, and Mean Absolute Error (MAE).

| Model | RMSE (lower is better) | R² (closer to 1 is better) | MAE (lower is better) |
| :--- | :--- | :--- | :--- |
| **Lasso Regression** | **0.1245** | **0.9081** | **0.0862** |
| XGBoost | 0.1411 | 0.8819 | 0.0932 |
| Linear Regression | 0.1449 | 0.8883 | 0.0935 |
| Random Forest | 0.1468 | 0.8722 | 0.0978 |

Based on these results, **Lasso Regression** was the best-performing model, demonstrating its effectiveness in handling a dataset with many features.

## Files in this Repository
* `House-Price-Prediction.ipynb`: The main Jupyter Notebook with all the code.
* `Project-Report.pdf`: The final project report in PDF format.
* `Action-Plan.pdf`: The project roadmap and timeline.
* `requirements.txt`: A list of all the necessary Python libraries to run the notebook.

## How to Run the Notebook
You can open the `House-Price-Prediction.ipynb` file directly in [Google Colab](https://colab.research.google.com/) or [Jupyter Notebook](https://jupyter.org/) to view and execute the code.
