# CS5710 Machine Learning — Homework 1 (Fall 2025)

**Student Name:** *M. Thanmayee*  
**Student ID:** *700776997*  
**Course:** CS5710 Machine Learning  
**University:** University of Central Missouri  

---

## 📌 Assignment Overview
This repository contains my solutions to **Homework 1** of CS5710 Machine Learning.  
The focus is on **function approximation, gradient descent, under/overfitting, and implementing linear regression**.  

For Q7, I implement **Linear Regression** using:
1. **Closed-form solution (Normal Equation)**
2. **Gradient Descent (GD)**  

Both methods are compared on synthetic data, and their results are visualized.

---

## 🚀 How to Run

### Requirements
- Python 3.8+
- Libraries: `numpy`, `matplotlib`

Install dependencies (if needed):

pip install numpy matplotlib


## 📊 Results & Analysis

### 1) Raw Data
Data follows:  
\[
y = 3 + 4x + \epsilon
\]  
with Gaussian noise.  

- The scatter plot shows a **clear linear trend** with random variation.

---

### 2) Closed-form Solution
Normal Equation:  
\[
\theta = (X^\top X)^{-1} X^\top y
\]

**Parameters:**
- Intercept ≈ **2.6908**
- Slope ≈ **4.1318**

- The red fitted line closely matches the data trend.

---

### 3) Gradient Descent Solution
- Initialized with \(\theta = [0,0]\)  
- Learning rate \(\eta = 0.05\)  
- Iterations = 1000  

**Parameters:**
- Intercept ≈ **2.6908**  
- Slope ≈ **4.1318**

- Gradient Descent converges to the **same solution** as the closed-form method.

---

### 4) Comparison
- Both Closed-form and GD produce **nearly identical lines**.  
- Confirms that MSE for linear regression is a **convex problem** with a unique global minimum.  

---

### 5) Loss Curve
- Loss starts **high** at \(\theta = [0,0]\).  
- It **rapidly decreases** during early iterations.  
- It **flattens out** after ~500 iterations, showing **convergence**.  

---

## 📝 Key Insights
- **Closed-form** is exact and efficient for small datasets.  
- **Gradient Descent** scales better to large datasets and complex models.  
- On this dataset, both converge to the **same optimum parameters**.  

**Short Summary:**  
We fit a linear model to synthetic data  
\[
y = 3 + 4x + \epsilon
\]  
The Normal Equation gave parameters \((2.6908,\,4.1318)\), and Gradient Descent converged to the same values after 1000 iterations.  
The loss curve confirmed convergence, and both methods produced identical fitted lines.

