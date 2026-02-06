# Gradient Descent for Linear Regression

**Name:** Rajavamshi Samudrala  
**Student ID:** 700774318  

---

## 📌 Problem Overview

Implement Linear Regression using two approaches:

1. Closed-form solution (Normal Equation)  
2. Gradient Descent (From scratch — no scikit-learn)

Compare both methods using the same synthetic dataset.

---

## 🧠 Dataset

Generate synthetic data using the following equation:

\[
y = 3 + 4x + \epsilon
\]

where:
- \( \epsilon \) is Gaussian noise  
- x values are sampled uniformly in \([0,5]\)  
- Total samples = **200**

---

## 🛠 Solution Approaches

### ➤ Closed-Form Solution (Normal Equation)

Compute:

\[
\theta = (X^TX)^{-1}X^Ty
\]

This yields the optimal intercept and slope directly using matrix algebra.

---

### ➤ Gradient Descent Implementation

Implemented from scratch with:
- Initial parameters: \( \theta = [0, 0] \)
- Learning rate: \( \eta = 0.05 \)
- Iterations: 1000

Tracks Mean Squared Error (MSE) over iterations and updates θ using:

\[
\theta := \theta - \eta \cdot \frac{2}{m} X^T(X\theta - y)
\]

---

## 📊 Output Visualizations

Notebook includes:

- Raw synthetic dataset (scatter plot)
- Fitted line from Normal Equation
- Fitted line from Gradient Descent
- Loss curve (MSE vs iterations)

---

## 📈 Results & Comparison

Both methods produce nearly identical estimates for the intercept and slope.  
This confirms that Gradient Descent converges to the same solution as the closed-form Normal Equation when configured with an appropriate learning rate and number of iterations.

---

## 📎 Files

- `Gradient_Descent_Linear_Regression.ipynb` — Colab notebook with full implementation  
- Plots generated in notebook (inline)

---
