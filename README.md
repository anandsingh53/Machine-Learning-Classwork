# 📘 Machine Learning Algorithms - Classwork implementation

This repository contains implementations and explanations of core **Machine Learning algorithms** applied to a real-world dataset: **ecommerce_sales_data.csv**.
All methods are implemented using **Python**, **pandas**, and **scikit-learn**, and are suitable for **college assignments, viva, and GitHub portfolios**.

---

## 📂 Dataset Used

**File Name:** `ecommerce_sales_data.csv`

### Columns Description:

| Column Name  | Description        |
| ------------ | ------------------ |
| Order Date   | Date of order      |
| Product Name | Name of product    |
| Category     | Product category   |
| Region       | Sales region       |
| Quantity     | Quantity sold      |
| Sales        | Total sales amount |
| Profit       | Profit earned      |

---

## 1️⃣ Data Collection

### 🔹 Objective

To load and inspect the dataset for further analysis and modeling.

### 🔹 Tools Used

* Python
* Pandas

### 🔹 Code Snippet

```python
import pandas as pd

df = pd.read_csv("ecommerce_sales_data.csv")
print(df.head())
```

### 🔹 Outcome

* Dataset successfully loaded
* Data ready for preprocessing and modeling

---

## 2️⃣ Multiple Linear Regression

### 🔹 Objective

To predict **Sales** using multiple independent variables such as:

* Quantity
* Category
* Region

### 🔹 Type

Supervised Learning – Regression

### 🔹 Key Concept

[ Sales = b_0 + b_1X_1 + b_2X_2 + b_3X_3 ]

### 🔹 Techniques Used

* One-Hot Encoding for categorical variables
* Train-Test Split

### 🔹 Outcome

* Continuous sales prediction
* Model evaluated using **MSE** and **R² Score**

---

## 3️⃣ Logistic Regression

### 🔹 Objective

To classify orders into:

* **High Profit (1)**
* **Low Profit (0)**

### 🔹 Type

Supervised Learning – Classification

### 🔹 Target Creation

```text
Profit ≥ Mean Profit → High Profit (1)
Profit < Mean Profit → Low Profit (0)
```

### 🔹 Evaluation Metrics

* Accuracy
* Confusion Matrix
* Precision, Recall, F1-score

### 🔹 Outcome

* Binary classification achieved
* Probabilistic interpretation using sigmoid function

---

## 4️⃣ Decision Tree

### 🔹 Objective

To classify orders as **High Profit** or **Low Profit** using a tree-based model.

### 🔹 Type

Supervised Learning – Classification

### 🔹 Splitting Criteria

* Gini Index
* Entropy (Information Gain)

### 🔹 Key Features

* Handles non-linear relationships
* Easy to interpret
* No need for feature scaling

### 🔹 Outcome

* Decision rules learned from data
* Controlled overfitting using max depth

---




