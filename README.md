# 🏡 House Price Prediction using Linear Regression

## Project Summary

This project demonstrates an end-to-end machine learning pipeline to predict residential housing sale prices. A **Linear Regression** model was developed, trained, and validated using Python and the Scikit-learn library to estimate property values based on key structural features.

---

## 🎯 Key Outcomes & Performance

The model was trained on an 80/20 data split and evaluated using industry-standard regression metrics:

| Metric | Value | Interpretation |
| :--- | :--- | :--- |
| **R² Score** | **0.767** | The model explains **76.7%** of the variability in house prices. |
| **RMSE (Root Mean Squared Error)** | **$40,536.19** | On average, the model's predictions are off by approximately **$40,536.19**. |

---

## Model Demonstration

The trained model was used to predict the price of a sample house not included in the training data:

* **Predicted Sale Price:** **$162,568.34**
* **Actual Sale Price:** **$145,000.00**

---

## 🛠️ Methodology & Technology Stack

### Data Preprocessing

* **Feature Selection:** Focused the model on **6 high-impact features** strongly correlated with price: *GrLivArea*, *OverallQual*, *TotalBsmtSF*, *GarageCars*, *FullBath*, and *YearBuilt*.
* **Missing Data Handling:** Utilized **median imputation** (`fillna(df.median())`) to ensure data completeness and model robustness.
* **Validation Check:** A **Residual Plot** was created, confirming that model errors were randomly distributed around the zero line, validating the use of the Linear Regression technique.

### Technologies

* **Python**
* **Pandas** (Data manipulation and cleaning)
* **NumPy** (Numerical operations)
* **Scikit-learn** (*LinearRegression*, *train\_test\_split*, and metrics)
* **Matplotlib** (Visualization for EDA and model evaluation)
### 🚀 Future Enhancements / Next Steps

To improve the model's performance and demonstrate a wider range of machine learning techniques, the following steps are planned:

1.  **Model Comparison (Classification):**
    * Implement and evaluate more advanced non-linear regression models, such as **Random Forest Regressor** or **XGBoost**.
    * The results will be compared against the Linear Regression baseline to determine the most effective algorithm for this dataset.

2.  **Advanced Feature Engineering (Categorical Data):**
    * Incorporate the rich information from the categorical features (e.g., `MSZoning`, `Neighborhood`, `HouseStyle`).
    * This will be done using methods like **One-Hot Encoding** to prevent these features from being discarded and to boost the model's predictive power.

3.  **Feature Scaling:**
    * Apply a **StandardScaler** to the numerical features (like `GrLivArea` and `TotalBsmtSF`).
    * Scaling features often improves the performance and convergence speed of linear models by ensuring no single feature dominates the calculation.

The complete code, step-by-step analysis, and all visualizations are contained in the **`my_projectinternship1 (2).ipynb`** notebook.
