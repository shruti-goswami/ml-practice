# Day 3 – Boston Housing Prices (Multiple Linear Regression)

## 📌 Problem
Predict the **median value of owner-occupied homes** (`MEDV`) in Boston suburbs using multiple features such as crime rate, number of rooms, tax rate, etc.  

This is a **Multiple Linear Regression** problem.  
Equation:  

\[
y = \beta_0 + \beta_1 x_1 + \beta_2 x_2 + \dots + \beta_n x_n
\]  

where `y = MEDV` and each `x_i` is one of the 13 features.

---

## 📂 Dataset
- Source: [Boston Housing Dataset (UCI)](https://archive.ics.uci.edu/ml/datasets/housing)  
- Shape: **506 rows × 13 features + target**  
- Target: `MEDV` → Median value of owner-occupied homes in $1000s  

---

## 🏡 Column Descriptions

| Column    | Description |
|-----------|-------------|
| **CRIM**      | Per capita crime rate by town |
| **ZN**        | Proportion of residential land zoned for lots over 25,000 sq. ft. |
| **INDUS**     | Proportion of non-retail business acres per town |
| **CHAS**      | Charles River dummy variable (1 if tract bounds river; 0 otherwise) |
| **NOX**       | Nitric oxides concentration (parts per 10 million) |
| **RM**        | Average number of rooms per dwelling |
| **AGE**       | Proportion of owner-occupied units built prior to 1940 |
| **DIS**       | Weighted distances to five Boston employment centres |
| **RAD**       | Index of accessibility to radial highways |
| **TAX**       | Full-value property-tax rate per $10,000 |
| **PTRATIO**   | Pupil–teacher ratio by town |
| **B**         | 1000(Bk - 0.63)² where Bk is the proportion of Black residents by town |
| **LSTAT**     | % lower status of the population |
| **MEDV**      | Median value of owner-occupied homes in $1000s (Target) |

---

## 🚀 Approach
1. **Data Exploration (EDA)**
   - Check distribution of target (`MEDV`)
   - Correlation heatmap between features and target
   - Pairplots (RM vs MEDV, LSTAT vs MEDV, etc.)

2. **Model Training**
   - Multiple Linear Regression (scratch + sklearn)
   - Train/test split
   - Fit model and extract coefficients

3. **Evaluation**
   - Metrics: Mean Squared Error (MSE), R² Score
   - Compare scratch vs sklearn implementation

4. **Visualization**
   - Residual plots
   - Predicted vs Actual values plot


## 📊 Visualization
- Correlation heatmap of all features
- Scatter plot of `RM` vs `MEDV` (positive relation)
- Scatter plot of `LSTAT` vs `MEDV` (negative relation)
- Predicted vs Actual home values

---

## 📁 Files in this folder
- `data/HousingData.csv` → dataset  
- `HousingPricePreduction.ipynb` → Jupyter Notebook with EDA + training  
- `BostHousingPricePrediction.py` → Python script version  
- `README.md` → This file  

---
