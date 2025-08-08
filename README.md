# MachineLearningAlgorithms# Horsepower vs Fuel Economy Prediction Using Simple Linear Regression

## Table of Contents
1. Problem Introduction  
2. Dataset  
3. Technologies Used  
4. Explanation  
5. Conclusion  

---

## 1. Problem Introduction  
A car manufacturer wants to analyze how a vehicle’s **horsepower** affects its **fuel economy** (miles per gallon – MPG).  
The hypothesis is that as **horsepower increases**, **fuel economy decreases**, because more powerful engines consume more fuel.  

**Variables:**  
- **Input (X):** Horsepower (HP)  
- **Output (Y):** Fuel Economy (MPG – Miles per Gallon)  

**Goals:**  
- Predict fuel economy based on horsepower  
- Help design vehicles balancing performance and efficiency  
- Assist customers in choosing fuel-efficient cars  

---

## 2. Dataset  

The dataset contains two main columns:  

| Car Model | Horsepower (HP) | MPG |
|-----------|----------------|-----|
| 1         | 70             | 38  |
| 2         | 90             | 35  |
| 3         | 110            | 32  |
| 4         | 150            | 28  |
| 5         | 200            | 22  |
| ...       | ...            | ... |

---

## 3. Technologies Used  
- **Python** for analysis and model building  
  - `pandas` – for data handling  
  - `numpy` – for numerical calculations  
  - `matplotlib` – for basic plots  
  - `seaborn` – for visualizing relationships  
  - `scikit-learn` – for regression modeling  

---

## 4. Explanation  

We use **Simple Linear Regression** to model the relationship:  

**Independent variable (X):** Horsepower  
**Dependent variable (Y):** Fuel Economy  

**Model Equation:**  
\[
MPG = m \times (Horsepower) + b
\]  

Where:  
- **m** = slope (rate at which MPG changes with horsepower)  
- **b** = intercept (MPG when horsepower is 0)  

**Expected outcome:** A **negative slope**, indicating that higher horsepower reduces fuel economy.  

**Steps:**  
1. Load the dataset with `pandas`  
2. Visualize with a scatter plot + regression line (`seaborn`)  
3. Train a `LinearRegression` model from `sklearn`  
4. Predict MPG for given horsepower values  

---

## 5. Conclusion  
This model will help:  
- Confirm the trade-off between power and efficiency  
- Guide engineering teams in tuning engines for optimal performance  
- Assist marketing teams in providing customers with accurate MPG predictions  

If the correlation is strong and negative, it will clearly show that **cars with higher horsepower consume more fuel**.  
