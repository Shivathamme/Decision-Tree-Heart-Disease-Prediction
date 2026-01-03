# Heart Disease Prediction using Decision Tree

This project demonstrates the use of a **Decision Tree Classifier** to analyze medical data and **predict the presence of heart disease**.  
The focus is on model interpretability, performance evaluation, and understanding how tree depth affects predictions.

---

## Problem Statement
To build a machine learning model that predicts whether a patient has heart disease based on clinical attributes such as age, cholesterol level, blood pressure, and heart rate.

---

## Dataset
- **Dataset:** Heart Disease Dataset  
- **Target Variable:** `target`  
  - `0` → No heart disease  
  - `1` → Heart disease present  
- **Features:** Age, sex, chest pain type, cholesterol, resting blood pressure, maximum heart rate, and other clinical attributes.

---

## Project Workflow
1. Data loading and exploration
2. Missing value check and data type inspection
3. Feature and target separation
4. Train–test split (80% training, 20% testing)
5. Decision Tree model training
6. Model evaluation using:
   - Accuracy score
   - Confusion matrix
   - Classification report
7. Hyperparameter experiments:
   - `max_depth`
   - `criterion` (Gini vs Entropy)
   - `min_samples_leaf`
8. Decision Tree visualization
9. Model comparison and final selection

---

## Model Experiments
Three Decision Tree models were trained using different tree depths:

| Model | max_depth | Training Accuracy | Testing Accuracy |
|------|----------|------------------|-----------------|
| Model 1 | 2 | 0.77 | 0.68 |
| Model 2 | 5 | 0.93 | 0.84 |
| Model 3 | None | 1.00 | 0.99 |

---

## Best Model Selection
Although the model with `max_depth=None` achieved the highest test accuracy, it showed signs of overfitting.  
The model with **`max_depth=5`** was selected as the best model because it provides a **good balance between accuracy and generalization**.

---

## Why Decision Trees?
- Handle both numerical and categorical data
- Capture non-linear relationships
- Easy to interpret and visualize
- Suitable for medical decision-making

---

## Tools & Libraries
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

---

## Conclusion
A moderately deep Decision Tree is effective for heart disease prediction.  
Controlling tree depth and leaf size helps prevent overfitting while maintaining strong predictive performance.


