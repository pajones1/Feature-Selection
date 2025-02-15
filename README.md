# 📊 Linear Regression and Model Evaluation Tutorial

## Overview
This tutorial explores **linear regression** and **model evaluation** using Python. You'll learn how to:
- Perform **simple and multiple linear regression**.
- Understand the **mathematical foundation** behind regression models.
- Evaluate model performance using **R², RMSE, and MAE**.
- Visualize regression results for deeper insights.

---

## 🔢 **Understanding Linear Regression**

Linear regression models the relationship between a dependent variable (**Y**) and one or more independent variables (**X**). The general equation is:

$$
Y = b_0 + b_1 X + \epsilon
$$

Where:
- **\( Y \)** → Dependent variable (what we predict)
- **\( X \)** → Independent variable (feature)
- **\( b_0 \)** → Intercept (value of \( Y \) when \( X = 0 \))
- **\( b_1 \)** → Slope (how much \( Y \) changes per unit increase in \( X \))
- **\( \epsilon \)** → Error term (unexplained variation)

### 📍 **Example: Simple Linear Regression**
Let's say we want to predict **house prices** (\$Y\$) based on **square footage** (\$X\$). If our model produces:

$$
Price = 50,000 + 200 \times (\text{Square Footage})
$$

- A **1 sq. ft. increase** adds **\$200** to the price.
- A house with **1,500 sq. ft.** would cost:

  $$
  Y = 50,000 + 200 \times 1500 = 350,000
  $$

---

## 📈 **Visual Representation of Linear Regression**
Linear regression finds the **best-fit line** through the data points.

```
       +--------------------------------+
       | House Price ($)                |
       |                                |
 450K  |     *                          |
 400K  |    **                          |
 350K  |   ***      Regression Line     |
 300K  |  ****   ----------------->     |
 250K  | *****                          |
       |--------------------------------|
            Square Footage (X)
```
_(A conceptual visualization of how regression fits a line to data.)_

---

## 🔎 **Model Evaluation Metrics**
Once we fit a model, we need to measure its accuracy. We use:

### **1️⃣ R² (Coefficient of Determination)**
Indicates how much **variance in \( Y \)** is explained by \( X \).

$$
R^2 = 1 - \frac{SS_{res}}{SS_{tot}}
$$

Where:
- \( SS_{res} \) = Sum of squared residuals (errors)
- \( SS_{tot} \) = Total variance in \( Y \)

- **\( R^2 = 1 \)** → Perfect prediction
- **\( R^2 = 0 \)** → Model explains nothing

| R² Value  | Interpretation                 |
|-----------|--------------------------------|
| **0.9+**  | Excellent fit (very accurate)  |
| **0.7-0.9** | Good fit                      |
| **0.5-0.7** | Moderate fit                   |
| **< 0.5** | Poor fit (weak model)          |

---

### **2️⃣ RMSE (Root Mean Squared Error)**
Measures the **average magnitude of prediction errors**:

$$
RMSE = \sqrt{\frac{1}{n} \sum (Y_{actual} - Y_{predicted})^2}
$$

Lower **RMSE** means **fewer large errors**.

---

### **3️⃣ MAE (Mean Absolute Error)**
Similar to RMSE but uses **absolute values** to avoid large errors skewing results:

$$
MAE = \frac{1}{n} \sum |Y_{actual} - Y_{predicted}|
$$

| Metric | Interpretation |
|--------|---------------|
| **Low RMSE** | Model makes small errors |
| **High RMSE** | Model has large errors |
| **Low MAE**  | Predictions are close to actual values |

---

## 🛠 **Technologies Used**
- **Python 3**
- **Pandas**: Data analysis
- **NumPy**: Mathematical operations
- **Scikit-Learn**: Machine learning (Linear Regression)
- **Matplotlib & Seaborn**: Data visualization

## 🚀 **Installation & Setup**
Ensure you have **Python 3** installed along with the required libraries:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## 🏃 **Running the Notebook**
Clone this repository and execute:
```bash
jupyter notebook "Formatted_Patrick_Jones_IOD_Lab_4.2.1.ipynb"
```

## 📊 **Example Model Output**
```plaintext
Linear Regression Model:
---------------------------------
Intercept: 5.2
Slope: 1.8
R² Score: 0.92 (92% variance explained)
RMSE: 2.13
MAE: 1.45
```
_(A visualization of regression results will be displayed in the notebook.)_

---

## 🌟 **Potential Enhancements**
- Implement **polynomial regression** for non-linear relationships.
- Add **interaction terms** for more complex models.
- Explore **Lasso/Ridge regression** to prevent overfitting.

---

This README is **formatted for GitHub Markdown** and will display correctly when uploaded. 🚀
