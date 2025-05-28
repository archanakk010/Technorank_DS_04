# 🏠 Predictive Modeling of House Prices using Machine Learning

##  Project Overview

This project aims to predict house prices using machine learning, with a focus on Support Vector Regression (SVR). A subset of the most relevant features was selected using Recursive Feature Elimination (RFE). The model was optimized through hyperparameter tuning using GridSearchCV, and its performance was evaluated on a test dataset.

---

##  Objective

- Identify key features affecting house prices using RFE.
- Build and optimize an SVR model using Scikit-learn.
- Evaluate the model with regression metrics such as R² Score, MSE, RMSE, and MAE.
- Understand the relationships between selected features and the target variable.

---

##  Problem Statement

Accurately predicting house prices is essential for stakeholders in the real estate market. Given multiple property attributes (e.g., size, construction quality, and year built), the challenge is to develop a machine learning model that can learn patterns from the data and predict house prices effectively.

---

##  Technologies Used

- Python
- Scikit-learn
- Pandas
- NumPy
- Matplotlib / Seaborn (for optional EDA)
- Jupyter Notebook

---

##  Methodology

1. **Feature Selection**  
   - Used Recursive Feature Elimination (RFE) to select 10 most impactful features.
   
2. **Model Building**  
   - Applied SVR (Support Vector Regression) with kernel tuning.
   
3. **Hyperparameter Tuning**  
   - GridSearchCV with 5-fold cross-validation.
   - Parameter Grid:
     - `C`: [0.1, 1, 10]
     - `epsilon`: [0.1, 0.2, 0.5]
     - `kernel`: ['linear', 'rbf']
   
4. **Model Evaluation Metrics**  
   - R² Score
   - Mean Squared Error (MSE)
   - Root Mean Squared Error (RMSE)
   - Mean Absolute Error (MAE)

---

##  Result

- **Best Parameters**: `{'C': 1, 'epsilon': 0.1, 'kernel': 'rbf'}`
- **Training R² Score**: 0.9305
- **Test R² Score**: 0.8917
- **MSE**: 0.0202  
- **RMSE**: 0.1422  
- **MAE**: 0.0967  

The SVR model exhibited strong performance with minimal overfitting and high accuracy.

---

##  Conclusion

This project successfully demonstrates how feature selection and hyperparameter tuning can enhance the performance of regression models. The SVR model achieved a high R² score on unseen test data, proving effective in capturing the underlying patterns of house price determinants. This approach can be extended to larger datasets or enhanced using ensemble models for production-grade systems.


