# 🏙️ Dubai Rental Price Prediction - Machine Learning Project

This project focuses on predicting property rental prices in Dubai using various machine learning models. It includes extensive data preprocessing, feature engineering, model training, and evaluation. The project also addresses common real-world challenges such as outliers, categorical encoding, and class imbalance.

## 📂 Dataset Overview

- **Source**: Property listings dataset
- **Target Variable**: Rent
- **Features**: Location, Area, Bedrooms, Bathrooms, Property Type, Furnishing, Date posted, etc.

## 🧹 Data Preprocessing

- Missing value imputation using median values.
- Categorical variables handled with Binary and One-Hot Encoding.
- Outliers capped using the IQR method.
- Rare categories grouped under "Other".
- Feature scaling using MinMaxScaler.

## 🧠 Feature Engineering

- Extracted Year, Month, and Day from the Posted_date column.
- Combined different encodings for categorical variables.
- Applied ExtraTreesRegressor and F-Regression to select the top 50 important features agreed upon by both methods.

## 🔍 Model Training & Hyperparameter Tuning

Models trained using GridSearchCV with 5-fold cross-validation:

- Linear Regression
- Ridge Regression
- Random Forest
- Decision Tree
- Gradient Boosting
- AdaBoost
- Bagging
- XGBoost

Top 3 models (by R²) used in ensemble techniques.

## 📊 Model Evaluation

Performance metrics used:

- R² (Coefficient of Determination)
- RMSE (Root Mean Squared Error)
- MAE (Mean Absolute Error)
- MSE (Mean Squared Error)

### 📌 Best Individual Models:

- **Random Forest**: R² ≈ 0.99, RMSE ≈ 11.2k
- **Bagging**: R² ≈ 0.99, RMSE ≈ 11.1k

## 🤝 Ensemble Learning

- **Voting Regressor**: Combines top 3 models with soft voting for better generalization.
- **Stacking Regressor**: Uses predictions from top 3 models as features for a final estimator (best performing model).

Both ensemble models outperformed individual ones.

## 📈 Visualizations

- Feature importance (ExtraTrees + F-Regression)
- Evaluation metric comparison charts
- Threshold tuning plot (for interpretability)

## 📌 Final Notes

This project demonstrates a complete ML pipeline from raw data to deployment-ready models. Special care was taken to ensure generalization, fairness (by handling rare categories), and robustness (handling outliers).

## 💡 Future Enhancements

- Integrate with a real-time dashboard or API.
- Extend to include price trends over time.
- Apply deep learning techniques for improved accuracy.


## Author
- **LinkedIn**: [Rayan Saleh](https://www.linkedin.com/in/rayan-saleh-b12a3132a)
- **GitHub**: [RayanAlDwlah](https://github.com/RayanAlDwlah)

Powered by passion for Machine Learning & Real-World Problem Solving 🚀
