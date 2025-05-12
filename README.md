#  Predictive Analysis Using Python – Housing Price Prediction

This project demonstrates how to perform **predictive analytics** using Python on a housing dataset. The goal is to explore, visualize, and model the relationship between house features and their prices using **linear regression**.

---

##  Dataset

- **Filename:** `Housing.csv`
- **Shape:** 545 rows × 13 columns
- **Attributes:**
  - `price`, `area`, `bedrooms`, `bathrooms`, `stories`, `mainroad`, `guestroom`, `basement`, `hotwaterheating`, `airconditioning`, `parking`, `prefarea`, `furnishingstatus`

---

## Project Workflow

### 1. Data Loading & Inspection

- Loaded the dataset using `pandas`
- Viewed top/bottom rows using `head()` and `tail()`
- Checked shape and descriptive statistics using `shape` and `describe()`
- Verified missing values with `isnull().sum()`

### 2. Exploratory Data Analysis (EDA)

- Visualized relationships using `seaborn.relplot()`:
  - `price` vs `area`
  - `price` vs `stories`
- Plotted correlation heatmap using `sns.heatmap()` to evaluate numeric correlations

### 3. Model Building: Linear Regression

- Separated features and target (`price`)
- Performed train-test split (`70%` train / `30%` test)
- Encoded categorical variables using `get_dummies()`
- Fitted a linear regression model using `sklearn.linear_model.LinearRegression`
- Made predictions and evaluated performance

### 4. Model Evaluation

- Used `r² score` to evaluate model performance on test set

---

## Requirements

1. Install required libraries with:

```bash
pip install pandas numpy seaborn scikit-learn matplotlib
```

 2. How to Run
- Clone the repository or download the notebook.
- Ensure Housing.csv is present in the same directory.
- Run the notebook using Jupyter or Google Colab.
