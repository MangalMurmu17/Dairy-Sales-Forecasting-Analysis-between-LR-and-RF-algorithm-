# 🥛 Forecasting Dairy Sales: A Comparative Analysis of Logistic Regression and Random Forest  

## 📌 Project Overview  
This project applies **Machine Learning** to forecast **dairy product sales** using real-world data. The focus is on comparing **Logistic Regression** and **Random Forest** models to identify the best approach for accurate sales prediction.  

The system analyzes factors such as **price, promotions, product details, and customer demand trends** to:  
- 📉 Reduce wastage in dairy supply chain  
- 📦 Optimize stock levels & reorder management  
- 💰 Improve business revenue through smarter forecasting  
- 📊 Provide insights into sales-driving factors  

---

## 📂 Dataset  
- **Source:** Kaggle (Dairy Sales Dataset)  
- **Shape:** 4,325 rows × 23 columns  
- **Features include:**  
  - Farm details (location, size, cows)  
  - Product details (ID, name, brand, shelf life)  
  - Sales data (quantity sold, price, total revenue)  
  - Inventory management (stock levels, reorder thresholds)  
  - Customer & sales channel info  
  - Dates: production, expiration, transaction  

---

## 🤖 Machine Learning Models Used  

### 1. Logistic Regression  
- Used for **sales category classification** (Low, Medium, High)  
- Relies on linear decision boundaries  
- Requires feature scaling (StandardScaler)  
- **Limitations:** struggles with nonlinear and complex patterns in dairy sales data  

### 2. Random Forest Classifier & Regressor  
- Ensemble of multiple decision trees (bagging + majority vote)  
- Handles nonlinear patterns & feature interactions  
- Provides **feature importance analysis** for interpretability  
- Achieved superior accuracy and stability compared to Logistic Regression  
- Extended to **RandomForestRegressor** for continuous sales forecasting (revenue prediction)  

---

## 🔬 Methodology  

1. **Data Preprocessing**  
   - Handle missing values  
   - Encode categorical variables (product, brand, sales channel)  
   - Extract temporal features (Year, Month, Quarter)  
   - Normalize features for Logistic Regression  

2. **Target Variable Creation**  
   - Sales classified into **Low / Medium / High categories**  

3. **Model Training**  
   - Train Logistic Regression & Random Forest models on training set (80:20 split)  
   - Cross-validation for stability  

4. **Model Evaluation**  
   - Metrics: Accuracy, Precision, Recall, F1-score  
   - Confusion Matrices for classification performance  
   - Feature importance ranking (Random Forest)  

5. **Business Insights**  
   - Identify key factors influencing dairy sales  
   - Recommendations for inventory & promotions  

---

## 📊 Results  

- ✅ **Random Forest outperformed Logistic Regression**  
  - Accuracy: **85.9% (RF) vs 58.4% (LR)**  
  - Cross-validation: **86.8% (RF) vs 57.0% (LR)**  
- 📈 **RandomForestRegressor** achieved **R² = 0.995**, proving excellent predictive power  
- 🔍 Top 10 most influential features identified for sales forecasting  
- 🏆 Random Forest demonstrated **better generalization, interpretability, and reliability**  

---

## 🖼️ Visuals

 🔹 **System Architecture**

 ![image alt](https://github.com/MangalMurmu17/Dairy-Sales-Forecasting-Analysis-between-LR-and-RF-algorithm-/blob/b9d79f17390f9cef0c1f1ce29c19c02c17eb3b90/System%20Architecture/LR.png)
 ![image alt](https://github.com/MangalMurmu17/Dairy-Sales-Forecasting-Analysis-between-LR-and-RF-algorithm-/blob/b9d79f17390f9cef0c1f1ce29c19c02c17eb3b90/System%20Architecture/RF.png)

 🔹 **Model Results & Graphs**

![image alt](https://github.com/MangalMurmu17/Dairy-Sales-Forecasting-Analysis-between-LR-and-RF-algorithm-/blob/731e9485a5e71634350b367c617af6fd8d3dc7f9/Results/Actual%20vs%20Predicted(counts)-RF%20classifier.png)
![image alt](https://github.com/MangalMurmu17/Dairy-Sales-Forecasting-Analysis-between-LR-and-RF-algorithm-/blob/731e9485a5e71634350b367c617af6fd8d3dc7f9/Results/Cross-Validation%20accuracy%20per%20fold.png)
![image alt](https://github.com/MangalMurmu17/Dairy-Sales-Forecasting-Analysis-between-LR-and-RF-algorithm-/blob/731e9485a5e71634350b367c617af6fd8d3dc7f9/Results/LR%20and%20RF%20Confusion%20Mstrix.png)
![image alt](https://github.com/MangalMurmu17/Dairy-Sales-Forecasting-Analysis-between-LR-and-RF-algorithm-/blob/731e9485a5e71634350b367c617af6fd8d3dc7f9/Results/Model%20accuracy%20comparison.png)
![image alt](https://github.com/MangalMurmu17/Dairy-Sales-Forecasting-Analysis-between-LR-and-RF-algorithm-/blob/731e9485a5e71634350b367c617af6fd8d3dc7f9/Results/RF%20regressor-Actual%20vs%20Predicted.png)

 🔹 **Insights**

![image alt](https://github.com/MangalMurmu17/Dairy-Sales-Forecasting-Analysis-between-LR-and-RF-algorithm-/blob/115731f52e2ac2b0ab69fcdeba73036a13e28fb2/Results/Top%2010%20RF%20feature%20importances.png)
![image alt](https://github.com/MangalMurmu17/Dairy-Sales-Forecasting-Analysis-between-LR-and-RF-algorithm-/blob/115731f52e2ac2b0ab69fcdeba73036a13e28fb2/Results/Forecasting%20Dairy%20Sales(RF%20regressor).png)

---

## 🛠️ Applications  
- 🛒 **Retail Stores** – Predict demand, avoid shortages  
- 🏭 **Dairy Processing Units** – Optimize production schedules  
- 🚚 **Supply Chain & Logistics** – Align distribution with demand forecasts  
- 🏪 **Supermarkets & Malls** – Plan promotions based on predicted trends  
- 📊 **Business Analysts** – Use insights for revenue growth & strategy  

---

## 🔮 Future Scope  
- Apply **advanced time-series models** (LSTM, Prophet) to capture seasonality  
- Expand to **multi-product forecasting** (all dairy items)  
- Integrate with **real-time sales pipelines** for live predictions  
- Develop a **dashboard / mobile app** for easy visualization of forecasts  
