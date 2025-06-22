# 🏦 Bank Loan Approval Prediction

> A Deep Learning-based system to predict personal loan approval using customer demographic and financial data.

---

## 🎯 Project Goal

The main goal of this project is to develop a robust neural network model that predicts whether a customer will be approved for a personal bank loan. The model uses customer features such as age, income, experience, account details, and more.

---

## 🧵 Dataset

- **Source**: [Universal Bank Dataset](https://www.kaggle.com/)
- **Target column**: `Personal Loan`  
  - `1` → Loan approved  
  - `0` → Loan not approved  
- **Features include**:
  - Age, Experience, Income, Family Size
  - Education Level
  - Mortgage Amount
  - Account Ownership (Securities, CD, Online, CreditCard)

---

## 🧽 Data Preprocessing

- Replaced negative `Experience` values with `Age - 23`
- Converted categorical fields like `Education`, `CD Account`, etc. to appropriate types
- Dropped `ZIP Code` due to limited variability
- Applied `StandardScaler` to numeric features
- Converted target and binary columns to boolean/categorical values

---

## 🧠 Models Implemented

| Model                 | Description                                                   | Accuracy |
|-----------------------|---------------------------------------------------------------|----------|
| Feedforward NN        | Basic ANN with ReLU activations and dropout regularization    | 97.1%    |
| TabNet Model          | Attention-based model for tabular data using PyTorch TabNet   | 98.5%    |
| Wide & Deep NN        | Combined wide linear and deep nonlinear components            | 97.6%    |

> The **TabNet model** achieved the highest accuracy.

---

## 📊 Exploratory Data Analysis

- Distribution plots for `Age`, `Income`, and `CCAvg`
- Countplots for categorical features (`Education`, `CreditCard`)
- Correlation heatmap to identify influential features
