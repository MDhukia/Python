# 🛒 Online Retail Cancellation Prediction

This project focuses on analyzing online retail customer transactions to **predict order cancellations** using machine learning.


## 📊 Overview

We engineered features from transaction data, segmented customers using **RFM + KMeans**, and applied multiple models to predict cancellations.  
The best-performing models were evaluated over time and interpreted through **feature importance**.


## 🔧 Tech Stack

- **Languages:** Python  
- **Libraries:** Pandas, Scikit-learn, XGBoost, Seaborn, Matplotlib  
- **Modeling:** Logistic Regression, Random Forest, Gradient Boosting, XGBoost  
- **Clustering:** KMeans for customer segmentation


## ⚙️ Workflow Summary

- Data Cleaning & Feature Engineering  
- Customer Segmentation (RFM + KMeans)  
- Model Training & Evaluation  
- Hyperparameter Tuning  
- Time-based Model Comparison  
- Feature Importance Analysis  


## ✅ Key Insights

- **Random Forest** gave the best overall performance  
- Top predictors: **DaysSincePrevPurchase**, **UnitPrice**, and **cluster features**  
- High-value customers with high cancellations require **proactive retention strategies**


## 💡 Recommendations

- Monitor customer segments for **high cancellation risk**  
- Optimize **order times** and **pricing strategies**  
- Deploy **predictive model** for early cancellation alerts
