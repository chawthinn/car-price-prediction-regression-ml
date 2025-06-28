# Used Car Price Prediction

This project builds a machine learning pipeline to predict used car prices using structured tabular data. It includes multiple regression models with a focus on accuracy, interpretability, and generalization.

## Project Overview

This project performs:
- Data preprocessing
- Exploratory Data Analysis (EDA)
- Feature engineering and encoding
- Model training with:
  - Linear Regression
  - Ridge Regression
  - XGBoost
  - LightGBM
- Evaluation and model selection using RMSE, MAE, and R²
- Model persistence

## Dataset

Used car dataset sourced from Kaggle. It includes features such as mileage, engine size, age, fuel type, and more.

## Notebook Outline

### Objective
### Dataset
### Import libraries

### 1. Data Preprocessing
- 1.1 Load the dataset and perform basic cleaning (handle missing values, duplicates)

#### Basic cleaning
- 1.2 Create a new feature: car_age = current_year - year
- 1.3 Drop irrelevant features like car_name if present
- 1.4 Convert categorical variables using One-Hot Encoding or Label Encoding
- 1.5 Normalize or scale the features

---

### 2. Exploratory Data Analysis
- 2.1 Visualize Price Distribution, Correlations, and Key Relationships
- 2.2 Boxplots for Categorical Features vs. selling_price
- 2.3 Histograms and Scatter Plots for Numerical Features

---

### 3. Model Building
- 3.1 Linear Regression
- 3.2 Ridge Regression
- 3.4 XGBoost Regressor (Optional: use LightGBM or any other advanced model)
- 3.5 LightGBM Regressor

---

### 4. Model Evaluation
- 4.1 Evaluate each model using: RMSE, MAE, R²

---

### 5. Model Selection
- 5.1 Select the best model based on lowest RMSE and highest R²

---

### 6. Save the Best Model
- 6.1 Use joblib or pickle to save the best-performing model

---

### Prepare for submission  
### References

## Tech Stack

- Python 3.10+  
- Pandas  
- NumPy  
- Scikit-learn  
- XGBoost  
- LightGBM  
- Matplotlib / Seaborn  
- Jupyter Notebook  

## How to Run

1. Clone this repo or open in Kaggle kernels

2. Install dependencies if running locally:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the notebook cell-by-cell

## Results

This project compared several regression models, including:

- Linear Regression  
- Ridge Regression  
- XGBoost  
- LightGBM  

All models were evaluated using RMSE, MAE, and R² on the test set. A comparison table summarizes their performance.

Among them, **LightGBM** and **XGBoost** delivered the best results in terms of accuracy and generalization.

The final model was saved using `pickle` for later use.

## Notes

This project is built to be modular and readable. Code is grouped by function, with each section focused on a specific part of the ML workflow.
