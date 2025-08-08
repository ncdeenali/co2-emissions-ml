# 🌍 CO₂ Emissions Prediction Using Machine Learning

---

## 📌 Overview
This project applies multiple regression models to predict **CO₂ emissions of vehicles** using features such as engine size, number of cylinders, fuel consumption, and fuel type.  
The goal is to evaluate and compare different machine learning algorithms to identify the most effective approach for accurate and scalable emissions forecasting.

---

## 🔍 Methods
### Data Exploration
- Visualized CO₂ emissions distribution and feature correlations.
- Checked for missing or inconsistent values (none found).
- Examined linear vs. non-linear feature relationships.

### Models Implemented
1. **Polynomial Regression**
2. **Random Forest Regressor**
3. **Gradient Boosting Regressor**
4. **XGBoost Regressor**

### Evaluation
- Train/test split: 80% / 20%
- Metrics:
  - Mean Absolute Error (MAE)
  - Mean Squared Error (MSE)
  - Root Mean Squared Error (RMSE)
  - R² Score
  - Computation Time (seconds)

---

## 📈 Model Comparison & Ranking

### 1️⃣ XGBoost – **Best Overall Model**
- **Performance:** Outperforms Gradient Boosting and Random Forest while showing strong generalization for smaller training sizes.
- **R²:** **98%** – highest explanatory power among all models.
- **Computation Speed:** Fastest at **23.83 seconds**, despite its advanced architecture.
- **Effectiveness Rank:** **#1** – Best trade-off between accuracy, generalization, and speed. Slight overfitting at larger training sizes but still the most effective.

### 2️⃣ Polynomial Regression
- **Performance:** Excellent baseline with lowest errors (MAE, MSE, RMSE) across all subsets and strong generalization.
- **R²:** 94%.
- **Computation Speed:** 38.48 seconds – efficient for small datasets.
- **Effectiveness Rank:** **#2** – Very effective for small datasets due to simplicity, but struggles with more complex, large-scale relationships.

### 3️⃣ Gradient Boosting
- **Performance:** Handles complex relationships better than Polynomial Regression, but suffers from higher errors and possible overfitting.
- **R²:** 96.6%.
- **Computation Speed:** Slowest at **302.22 seconds**.
- **Effectiveness Rank:** **#3** – Scalable but less efficient due to high errors and training time.

### 4️⃣ Random Forest Regressor
- **Performance:** Highest errors and largest train-test loss gaps, indicating overfitting.
- **R²:** 96.6%.
- **Computation Speed:** Moderate at **65.13 seconds**.
- **Effectiveness Rank:** **#4** – Least effective for this project.

---

## 🏆 Final Verdict
**XGBoost** is the recommended model for CO₂ emissions prediction in this dataset.  
It delivers the best combination of:
- **High accuracy**
- **Fast computation time**
- **Strong scalability**

---

## 📜 Conclusion
The results show that while simpler models like Polynomial Regression perform well for small datasets, advanced algorithms such as **XGBoost** are better suited for large-scale, real-world CO₂ emissions prediction tasks.  
Future improvements could include:
- Hyperparameter tuning for XGBoost and Gradient Boosting
- Additional vehicle attributes to improve prediction accuracy
- Feature engineering to capture more complex patterns

---
