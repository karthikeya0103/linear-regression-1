# Ecommerce Customer Spend Prediction using Linear Regression

This project demonstrates how to perform **exploratory data analysis**, feature engineering, and build a **Linear Regression model** to predict customer spending behavior based on their digital interaction patterns on an ecommerce platform.

---

##  Dataset: `Ecommerce.csv`

The dataset contains user-level analytics from an ecommerce website. Each record represents a unique user along with the following features:

| Feature Name           | Description                                 |
|------------------------|---------------------------------------------|
| `Email`                | User email ID (not used for modeling)       |
| `Address`              | User address (not used for modeling)        |
| `Avatar`               | Profile image label (categorical, unused)   |
| `Avg. Session Length`  | Average duration of a browsing session      |
| `Time on App`          | Time spent on the mobile app                |
| `Time on Website`      | Time spent on the website                   |
| `Length of Membership` | Number of years the user has been active    |
| `Yearly Amount Spent`  |  **Target variable** — annual spending     |

---

##  Project Objective

> Predict the **Yearly Amount Spent** by a user using their behavioral and engagement metrics.

---

##  Machine Learning Workflow

-  Load and inspect the dataset
-  Perform EDA using `seaborn` and correlation heatmaps
-  Identify key predictive features
-  Split data into training and testing sets
-  Build and evaluate a **Linear Regression** model
-  Analyze residuals to validate model assumptions

---

## Model Performance

| Metric | Value |
|--------|-------|
| **R² Score** | 0.978 |
| **Mean Squared Error** | 109.86 |

**Key Predictors**:
- `Length of Membership`
- `Time on App`
- `Avg. Session Length`

---

## Files

| File | Description |
|------|-------------|
| `Ecommerce.csv` | Raw dataset used for analysis |
| `linear_regression.ipynb` | Jupyter notebook performing full EDA and model training |
| `README.md` | Project overview and documentation |

---

## Key Learnings

- **Feature importance matters**: Time on app had significantly more predictive power than website time.
- **Linear regression assumptions**: Residual analysis confirmed the model is well-suited for this use case.
- **Real-world use case**: Understanding spending behavior can drive marketing and UX strategies in ecommerce.

---

## How to Run

1. Clone the repository
2. Install dependencies:

```bash
pip install pandas matplotlib seaborn scikit-learn
```

3.Launch Jupyter:
```bash
jupyter notebook
```
4.Open and run linear_regression.ipynb
