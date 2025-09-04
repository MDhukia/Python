# 🛒 Customer Personality Analysis  

## 📌 Overview
This project analyzes customer data from a marketing campaign to understand customer behavior, segment them into meaningful clusters, and predict high-value spenders using machine learning models.  

The analysis helps businesses:  
- Understand **customer demographics and behavior**  
- Build **customer segmentation** for targeted marketing  
- Predict **high-spending customers** for revenue optimization  

---


## 🛠️ Project Workflow

### 1. Data Preprocessing
- Handled missing values (`Income`)  
- Feature engineering:  
  - **Age** (from `Year_Birth`)  
  - **Enrollment_Duration** (days since first purchase)  
- Removed unnecessary columns  

### 2. Exploratory Data Analysis (EDA)
- Distribution plots (histograms, boxplots) for key features  
- Correlation heatmaps  
- Outlier detection  

### 3. Customer Segmentation (Clustering)
- **KMeans Clustering** with scaled features  
- **Elbow Method** and **Silhouette Score** to determine optimal k  
- Cluster profiling to analyze spending patterns and demographics  

### 4. Prediction Models
Target: **High Spender (binary)**  
- Defined based on total product spending above the median  
- Models used:  
  - Logistic Regression  
  - Random Forest Classifier  
  - XGBoost Classifier  

### 5. Evaluation
- Accuracy, Precision, Recall, F1-score  
- Confusion Matrices  
- Feature importance visualization (Random Forest & XGBoost)  

---

## 📈 Visualizations
- Distribution of Age, Income, Recency  
- Boxplots for outlier detection  
- Correlation heatmap of numerical features  
- Elbow vs Silhouette curve for clustering  
- Feature importance plots  

---

## 🚀 Tech Stack
- **Language:** Python  
- **Libraries:**  
  - Data Analysis: `pandas`, `numpy`  
  - Visualization: `matplotlib`, `seaborn`  
  - Machine Learning: `scikit-learn`, `xgboost`  

---

## 🔍 Results
- **Customer Segmentation:** Identified 4 distinct clusters with unique spending and engagement behavior  
- **Prediction Models:**  
  - Logistic Regression – simple baseline, interpretable  
  - Random Forest – strong performance with feature insights  
  - XGBoost – best accuracy and generalization  




