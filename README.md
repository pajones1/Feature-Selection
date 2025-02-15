# Linear Regression and Model Evaluation Tutorial 📊

## Overview
This tutorial focuses on **linear regression analysis** and **model evaluation** using Python. It provides a step-by-step guide on how to:
- Perform **simple and multiple linear regression**.
- Understand the **mathematical foundation** of regression.
- Evaluate model performance using **R² (coefficient of determination), RMSE (Root Mean Squared Error), and MAE (Mean Absolute Error)**.
- Visualize regression results for deeper insights.

## Key Topics Covered
- Understanding **linear regression equations**.
- Implementing **least squares regression**.
- Evaluating regression models with statistical metrics.
- Visualizing relationships between dependent and independent variables.

---

## 📌 **Understanding Linear Regression**
Linear regression is one of the most fundamental predictive modeling techniques. It assumes a **linear relationship** between independent variables (**X**) and a dependent variable (**Y**).

### 🔹 **Mathematical Formula**
For **simple linear regression**, where there is only one independent variable, the equation is:

\[
Y = b_0 + b_1 X + \epsilon
\]

Where:
- \( Y \) = Dependent variable (target)
- \( X \) = Independent variable (predictor)
- \( b_0 \) = Intercept (value of Y when X = 0)
- \( b_1 \) = Slope (rate of change in Y per unit change in X)
- \( \epsilon \) = Error term (difference between actual and predicted values)

For **multiple linear regression** with multiple predictors:

\[
Y = b_0 + b_1 X_1 + b_2 X_2 + ... + b_n X_n + \epsilon
\]

Where \( X_1, X_2, ..., X_n \) are multiple independent variables.

---

## 📌 **Evaluating Model Performance**
Once a regression model is built, we must **assess its accuracy** using various metrics.

### 🔹 **R² (Coefficient of Determination)**
R² tells us **how well the model explains the variability** in the target variable. It is calculated as:

\[
R^2 = 1 - \frac{SS_{res}}{SS_{tot}}
\]

Where:
- \( SS_{res} \) = Sum of squared residuals (difference between actual and predicted values)
- \( SS_{tot} \) = Total sum of squares (variance in actual values)

- **R² = 1** → Perfect fit (model explains all variance)
- **R² = 0** → Model explains none of the variance

### 🔹 **RMSE (Root Mean Squared Error)**
Measures the standard deviation of residuals (prediction errors). Lower RMSE indicates a better model.

\[
RMSE = \sqrt{\frac{1}{n} \sum (Y_{actual} - Y_{predicted})^2}
\]

### 🔹 **MAE (Mean Absolute Error)**
MAE calculates the average absolute difference between actual and predicted values:

\[
MAE = \frac{1}{n} \sum |Y_{actual} - Y_{predicted}|
\]

MAE is less sensitive to large errors than RMSE, making it useful when large deviations should not be overly penalized.

---

## 🔧 **Technologies Used**
- **Python 3**
- **Pandas**: Data manipulation and analysis
- **NumPy**: Mathematical operations
- **Scikit-Learn**: Machine learning (Linear Regression)
- **Matplotlib & Seaborn**: Data visualization

## 🛠 **Installation & Setup**
### Prerequisites
Ensure you have **Python 3** installed along with the required libraries:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
