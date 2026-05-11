# Retail Sales Forecasting: Predictive Analytics for Outlet Performance

## 📌 Project Overview
This project focuses on building a robust predictive model to forecast sales for a major retail chain (BigMart). By analyzing product attributes (weight, visibility, type) and outlet characteristics (size, location, establishment year), the goal is to identify the key drivers of sales and provide actionable insights for inventory management and revenue optimization.

## 📊 Business Insights
Through a thorough Exploratory Data Analysis (EDA), two primary insights were identified to drive operational efficiency:

### 1. The Impact of Outlet Type on Sales Consistency
* **Insight:** Supermarket Type 3 consistently outperforms other outlet types (Grocery Stores and Type 1/2) in terms of average sales volume. This suggests that the larger scale and operational model of Type 3 locations drive higher customer engagement.
* **Strategic Recommendation:** Scaling the inventory management strategies of Type 3 to other outlets could significantly boost overall revenue.

### 2. Item Visibility Paradox
* **Insight:** The analysis revealed that many products with recorded visibility of "0.0" were still generating sales, which indicated a data inconsistency. After correcting this and applying a "Minimum Presence" imputation, we found that visibility significantly impacts sales for daily essentials like "Dairy" and "Bread."
* **Strategic Recommendation:** Optimizing shelf placement for high-turnover daily products can drive impulse purchases and increase average basket size.

## 🤖 Model Summary & Evaluation
The project involved a complete machine learning pipeline, including data cleaning, feature engineering, and advanced regression modeling.

* **The Pipeline:**
    * **Preprocessing:** Missing values were handled using specialized imputation (Mean for weight, Mode for outlet size).
    * **Encoding:** Used **Ordinal Encoding** for tiered locations and **One-Hot Encoding** for categorical features.
    * **Scaling:** Numerical features were standardized for model stability.

* **Final Model Performance:**
    * **Primary Model:** Tuned Random Forest Regressor (via GridSearchCV).
    * **Key Metrics:**
        * **Test R² Score:** **0.604** (A balanced and reliable score for retail forecasting).
        * **Mean Absolute Error (MAE):** ~727 (Average deviation in sales prediction).

---
*This project was developed to showcase data science skills in predictive modeling, data cleaning, and business analytics.*
