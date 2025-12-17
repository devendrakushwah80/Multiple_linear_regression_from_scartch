# 📈 Multiple Linear Regression From Scratch (NumPy)

This project demonstrates how **Multiple Linear Regression (MLR)** can be implemented **from scratch using NumPy**, without relying on `sklearn`'s regression models. The notebook focuses on understanding the **mathematics, matrix operations, and evaluation metrics** behind linear regression.

---

## 🚀 Project Overview

The notebook covers:

* Building a **custom Multiple Linear Regression class**
* Training the model using the **Normal Equation (Closed-Form Solution)**
* Performing **Train–Test Split**
* Making predictions on unseen data
* Evaluating model performance using standard regression metrics

This is ideal for:

* Learning ML fundamentals
* Interview preparation
* Understanding what happens behind `LinearRegression()` in sklearn

---

## 🧠 Theory Used

The hypothesis function:

[ \hat{y} = Xw + b ]

Where:

* `X` → Feature matrix
* `w` → Weights (coefficients)
* `b` → Bias (intercept)

### 🔢 Normal Equation

[ \theta = (X^T X)^{-1} X^T y ]

This approach avoids gradient descent and directly computes optimal parameters.

---

## 🛠️ Implementation Details

### Custom Class

```python
class My_MLR:
    def fit(self, X_train, y_train):
        # uses normal equation
    def predict(self, X_test):
        # returns predictions
```

* Bias term is added manually using a column of ones
* Uses pure **NumPy matrix operations**

---

## 📊 Model Evaluation Metrics

The following metrics are calculated:

* **MAE (Mean Absolute Error)**
* **MSE (Mean Squared Error)**
* **RMSE (Root Mean Squared Error)**
* **R² Score**
* **Adjusted R² Score**

### Adjusted R² Formula

[ Adjusted\ R^2 = 1 - (1 - R^2) \times \frac{n - 1}{n - p - 1} ]

Where:

* `n` = number of samples
* `p` = number of features

---

## 🧪 Workflow

1. Import libraries
2. Define custom regression class
3. Load dataset
4. Perform train–test split
5. Train model using `.fit()`
6. Predict using `.predict()`
7. Evaluate using regression metrics
---

## 📁 File Structure

```
📦 Multiple-Linear-Regression-From-Scratch
 ┣ 📜 Multiple_linear_regression_from_scartch.ipynb
 ┣ 📜 README.md
 ┗ 📜 requirements.txt
```

---

## ✅ Key Learnings

* How OLS works internally
* Role of matrix multiplication in ML
* Why `(XᵀX)` can become singular
* Difference between R² and Adjusted R²
* When closed-form solution is not preferred (large data)

---

## 🧑‍💻 Author

**Devendra Kushwah**
Machine Learning Enthusiast | Python Developer

---

⭐ If you found this helpful, consider starring the repo!
