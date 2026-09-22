# 🏠 House Price Prediction using XGBoost

![Python](https://img.shields.io/badge/Python-3.12-blue?logo=python) ![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-orange?logo=scikitlearn) ![XGBoost](https://img.shields.io/badge/XGBoost-green) ![License](https://img.shields.io/badge/License-MIT-blue)

## 📌 Overview

This project predicts house sale prices using **XGBoost Regression**. It demonstrates a complete machine learning workflow, including data preprocessing, missing value imputation, categorical feature encoding, model training, evaluation, visualization, and feature importance analysis.

## 📊 Model Performance

The initial XGBoost model achieved the following results on the held-out test set:

| **Metric** | **Score** |
| ---------- | --------- |
| MAE        | 15,971.10 |
| RMSE       | 25,715.85 |
| R² Score   | 0.9138    |
| MAPE       | 9.47%     |

## Workflow

1. Load Dataset
2. Separate Features and Target
3. Train-Test Split
4. Identify Numerical and Categorical Features
5. Handle Missing Values
6. One-Hot Encode Categorical Features
7. Combine Numerical and Encoded Features
8. Train XGBoost Regressor
9. Generate Predictions
10. Evaluate Model
11. Visualize Results
12. Analyze Feature Importance

## 📂 Dataset

* **House Prices: Advanced Regression Techniques**
* Source: Kaggle
* Training dataset contains **1,460 rows and 81 columns**
* 80 input features
* Target variable: `SalePrice`

The dataset contains numerical and categorical information about residential properties, including house quality, living area, garage information, basement characteristics, neighborhood, and other property attributes.

## 🚀 Features

* Missing value handling
* Median imputation for numerical features
* Most-frequent imputation for categorical features
* One-Hot Encoding
* Train-Test Split
* XGBoost Regression
* Regression model evaluation
* Actual vs Predicted visualization
* Residual analysis
* Prediction error distribution
* Feature Importance Analysis

## 📊 Evaluation Metrics

* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)
* R² Score
* Mean Absolute Percentage Error (MAPE)

## 🛠 Technologies Used

* Python
* Pandas
* NumPy
* Scikit-Learn
* XGBoost
* Matplotlib
* Jupyter Notebook

## 📈 Actual vs Predicted

The Actual vs Predicted plot compares the model's predicted house prices with their actual sale prices.

![Actual vs Predicted](images/actual_vs_predicted.png)

## 📉 Residual Plot

The residual plot shows the difference between the actual and predicted house prices.

![Residual Plot](images/residual_plot.png)

## 📊 Prediction Error Distribution

This visualization shows the distribution of prediction errors produced by the model.

![Prediction Error Distribution](images/error_distribution.png)

## ⭐ Feature Importance

Feature importance shows which features were most influential in the trained XGBoost model.

![Feature Importance](images/feature_importance.png)

The most important feature in the model was **OverallQual**, followed by features including **GarageCars**, **RoofMatl_CompShg**, **ExterQual_Ex**, and **BsmtQual_Ex**.

## 📁 Files

* `House_Price_Prediction_XGBoost.ipynb`
* `requirements.txt`
* `images/`

  * `actual_vs_predicted.png`
  * `residual_plot.png`
  * `error_distribution.png`
  * `feature_importance.png`

> The Kaggle dataset is not included in this repository. Download the dataset from Kaggle and place `train.csv` in the appropriate dataset directory before running the notebook.

## 📌 Conclusion

This project demonstrates an end-to-end **machine learning regression workflow** for predicting house sale prices using XGBoost.

The initial model achieved an **R² score of 0.9138** and a **MAPE of 9.47%** on the held-out test set. Feature importance analysis showed that **OverallQual** was the most influential feature among the encoded features used by the model.

Future improvements include hyperparameter tuning, cross-validation, early stopping, feature engineering, and model explainability using SHAP.

## 👩‍💻 Author

**Samiha Sarwar**

GitHub: SamihaAlii
