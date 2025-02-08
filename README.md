# **Customer Churn Prediction**

## **Project Overview**
This project aims to predict customer churn using machine learning techniques. The dataset includes customer details, subscription information, and churn status. The best-performing model, **Gradient Boosting**, achieved an **85% accuracy** after feature engineering and hyperparameter tuning.

## **Dataset**
The dataset contains:
- **Customer Information**: Gender, age, partners, dependents.
- **Service Details**: Internet type, phone services, tech support, streaming services.
- **Billing & Contract**: Monthly charges, contract type, payment method, paperless billing.
- **Churn Status**: Whether the customer left the service.

## **Approach**
1. **Exploratory Data Analysis (EDA)**
   - Identified patterns in customer behavior.
   - Visualized churn trends using **Seaborn & Matplotlib**.

2. **Data Preprocessing**
   - One-hot encoding for categorical variables.
   - Scaled numerical features for better performance.
   - **SMOTE** applied to balance class distribution.

3. **Model Training & Evaluation**
   - Tested multiple models: **Logistic Regression, Random Forest, XGBoost, Gradient Boosting**.
   - **Gradient Boosting** performed best (**85% accuracy, 0.85 ROC-AUC**).
   - **GridSearchCV** used for hyperparameter tuning.

4. **Feature Importance Analysis**
   - Key features: **Contract type, tenure, payment method, online security**.
   - Month-to-month contracts had the highest churn rates.

## **Technologies Used**
- **Python** (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn)
- **Machine Learning Models** (Gradient Boosting, XGBoost, Random Forest, Logistic Regression)
- **SMOTE** for handling class imbalance
- **GridSearchCV** for hyperparameter optimization

## **Results & Insights**
- Customers with **month-to-month contracts** are more likely to churn.
- **Online security, tenure, and payment method** play a crucial role in churn prediction.
- Optimized **Gradient Boosting model** achieved **85% accuracy** with **0.85 ROC-AUC**.

## **Project Files**
📄 `Data.csv` - Dataset 
📄 `cleaned_data.csv` - Cleaned Dataset 
📄 `churn_prediction.ipynb` - Main notebook containing the full workflow  
📄 `xgboost_model.pkl` - Trained Model 

## **Contributing**
Feel free to submit issues or pull requests to improve the model or add new insights!

## **License**
This project is open-source and available under the **MIT License**.
