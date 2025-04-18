# Medical Cost Regression Using Machine Learning  
**Author:** Eric Meyer

**Date:** 4/17/2025

**My Project Notebook:** [ML Final Project Juptyer Notebook](https://github.com/ericmeyer1/ml_regression_eric/blob/main/ml_regression_eric.ipynb)

---

## Overview  
This project applies linear and polynomial regression techniques to predict individual medical costs based on features like age, BMI, smoking status, and more. Using the popular **Medical Cost Personal Dataset**, the goal was to evaluate how well linear models could capture relationships between patient attributes and medical charges, and explore ways to improve prediction performance.

We compared baseline linear regression with pipelines using scaling and polynomial feature engineering.

---

## Project Files  
- **Jupyter Notebook** – Full implementation with code, visualizations, and reflections.  
- **Charts and Visuals** – Included in the notebook for EDA and model evaluation.  

---

## Clarity & Organization  
**Strengths:**  
- The notebook is structured into clearly labeled sections: data exploration, preprocessing, modeling, evaluation, and reflection.  
- Visualizations (scatter plots, histograms, correlation heatmaps) make trends in the data easy to understand.  

**Areas for Improvement:**  
- Could include more visual aids during model evaluation (e.g., residual plots or prediction vs. actual plots).  
- Add a table of contents in the markdown for navigation ease in long notebooks.

---

## Feature Selection & Justification  
**Strengths:**  
- All provided features (age, sex, BMI, children, smoker, region) were retained and used after encoding.  
- Feature relationships were explored with pairplots and correlation heatmaps.

**Areas for Improvement:**  
- Consider dropping or transforming features with minimal correlation in future versions.  
- Create more interaction terms or domain-specific composite features.

---

## Model Performance & Comparisons  

**Models Used:**  
- **Linear Regression (Baseline)**  
- **Pipeline with StandardScaler + Linear Regression**  
- **Pipeline with Polynomial Features (degree=3)**  

**Performance Metrics:**  
- **Linear Regression R²:** 0.7811  
- **Pipeline R²:** 0.7811  
- **Polynomial Pipeline R²:** 0.8640  

**Strengths:**  
- Polynomial regression significantly improved predictive power by modeling nonlinear relationships.  
- Pipelines helped organize transformations and improved reproducibility.

**Areas for Improvement:**  
- Incorporate regularization (Lasso, Ridge) to limit overfitting with polynomial models.  
- Add cross-validation to better assess model generalizability.

---

## Reflection Quality  

**What Worked:**  
- Smoking status and BMI were highly predictive of cost.  
- Polynomial regression captured complexity missed by linear models.

**Limitations:**  
- Risk of overfitting with high-degree polynomial terms.  
- Small dataset size limits robustness.

**Next Steps:**  
- Try ensemble models like Random Forest or Gradient Boosting.  
- Tune polynomial degree with `GridSearchCV`.  
- Add SHAP or permutation importance for model explainability.  

---

## Setup Instructions  
To run this project locally:  

1. Clone the repository  

- git clone https://github.com/ericmeyer1/ml_regression_eric.git 

