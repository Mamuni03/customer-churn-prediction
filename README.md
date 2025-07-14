# customer-churn-prediction

# Customer Churn Prediction

This project focuses on predicting customer churn using machine learning techniques. Churn prediction is crucial for businesses to retain valuable customers and minimize losses. The dataset used in this project is **imbalanced**, and thus special care was taken to balance it using **SMOTE** (Synthetic Minority Over-sampling Technique).

## 📌 Project Objectives

- Understand the factors affecting customer churn through **Exploratory Data Analysis (EDA)**
- Handle imbalanced classes using **SMOTE**
- Build and evaluate various **Machine Learning models**
- Compare model performance before and after SMOTE
- Identify the best-performing model based on the **F1-score**

---

## 📂 Dataset

The dataset contains customer information such as:

customerID', 'gender', 'SeniorCitizen', 'Partner', 'Dependents',
       'tenure', 'PhoneService', 'MultipleLines', 'InternetService',
       'OnlineSecurity', 'OnlineBackup', 'DeviceProtection',
       'TechSupport', 'StreamingTV', 'StreamingMovies', 'Contract',
       'PaperlessBilling', 'PaymentMethod', 'MonthlyCharges',
       'TotalCharges', 'Churn'
**Note**: The target variable `Churn` is imbalanced.

---

## 📊 Exploratory Data Analysis (EDA)

- Checked for missing values and data types
- Visualized churn distribution (imbalance confirmed)
- Perform both univariate and bivariate analysis
- Analyzed categorical and numerical features
- Plotted correlation heatmap
- Derived insights from churn vs non-churn groups

---

## ⚖️ Handling Imbalanced Dataset

The dataset was imbalanced, leading to biased performance toward the majority class.

### ✅ Technique Used: **SMOTE**
- SMOTE was applied to oversample the minority class
- Helped improve the model’s ability to detect churned customers
- Perform hyperparameter tuning using optuna
---

## 🤖 Models Trained

| Model                 | F1 Score (Before SMOTE) | F1 Score (After SMOTE) |
|----------------------|-------------------------|------------------------|
| Random Forest        | 76.79%                  | **77.13%**             |
| XGBoost              | 76.60%                  | 76.60%                 |
| Decision Tree        | 76.30%                  | 76.30%                 |
| Logistic Regression  | 74.06%                  | 74.06%                 |

- Classification reports were printed for all models
- **Random Forest** performed the best after SMOTE application

---

## 🏆 Best Model: Random Forest

- **F1 Score**: **77.13%**
- Balanced precision and recall
- Robust to overfitting
- Interpretable and easy to tune

---

## 📈 Evaluation Metric

- **F1 Score** was used to evaluate model performance, especially suitable for imbalanced datasets
- **Classification Report** was used to assess precision, recall, and support for both classes

---

## 🧪 Tools and Libraries

- Python
- Pandas, NumPy
- Matplotlib, Seaborn (for EDA)
- Scikit-learn (for ML models and SMOTE)
- XGBoost
  
---

## 📌 Conclusion

- The dataset was successfully analyzed and balanced
- Random Forest classifier performed best with a post-SMOTE **F1-score of 77.13%**
- The project demonstrates effective handling of class imbalance and model selection for churn prediction


