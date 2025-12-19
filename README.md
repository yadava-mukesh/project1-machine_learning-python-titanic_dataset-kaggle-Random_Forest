# Titanic Survival Prediction using Random Forest 🛳️🌲

## 📌 Project Overview
This project focuses on predicting passenger survival on the **Titanic dataset (Kaggle)** using a **Random Forest Classifier**. The objective is to build a robust, non-linear model, tune it using cross-validation, and interpret results through feature importance.

## 📊 Dataset
* **Source:** Kaggle Titanic Dataset
* **Total Rows:** 891
* **Target Variable:** `Survived` (0 = Did not survive, 1 = Survived)

## 🔧 Data Preprocessing
* Handled missing values (Age, Embarked)
* Encoded categorical variables (Sex, Embarked)
* Selected relevant features for modeling
* Train–test split with cross-validation

📌 *Feature scaling was not applied, as Random Forest is a tree-based model and does not require it.*

## 🤖 Model: Random Forest Classifier
* Captures non-linear relationships and feature interactions
* Robust to outliers and skewed data
* Performs well on structured/tabular datasets

### 🔍 Hyperparameter Tuning
* Used **GridSearchCV** to optimize:

  * `n_estimators`
  * `max_depth`
  * `min_samples_split`
  * `min_samples_leaf`

## 📈 Model Performance
* **Training Accuracy:** ~97.6%
* **Cross-Validation Accuracy:** ~81.3%
* **Test Accuracy:** ~83.2%

The model shows strong generalization on unseen data, with slight overfitting that is common for ensemble tree models.

## ⭐ Feature Importance
* Analyzed important features using:

  ```python
  best_estimator_.feature_importances_
  ```
* Helped identify key factors influencing passenger survival

## 🛠️ Tech Stack
* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn

## 🧠 Key Learnings
* Tree-based models do not require feature scaling
* Importance of cross-validation for model evaluation
* How hyperparameter tuning improves model performance
* Interpreting feature importance for explainability

## 🚀 Future Improvements
* Advanced feature engineering (FamilySize, IsAlone, Title extraction)
* Try Gradient Boosting / XGBoost
* Optimize for recall or F1-score instead of accuracy

## 📬 Contact
Feel free to connect with me on **LinkedIn** to discuss data analytics, machine learning projects, or learning journeys.
