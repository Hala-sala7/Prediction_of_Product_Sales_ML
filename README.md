# Prediction of Product Sales

## Analyzing Product and Store Attributes to Predict Sales

**Author**: Hala Salah

### Business Problem:
The goal of this project is to help retailers understand the properties of products and outlets that play crucial roles in increasing sales. By building a predictive model, we aim to forecast the sales of each product at a particular outlet.

## Exploratory Data Analysis (EDA)

During the EDA phase, several visualizations were created to understand the distribution of data and identify trends:

### 1. Item Visibility Distribution
Most products have low visibility (concentrated between 0.00 and 0.10), indicating that only a few items get premium shelf space.
<img width="571" height="433" alt="download" src="https://github.com/user-attachments/assets/d7c2a969-7bf0-4956-8a12-87f5acc0fe56" />
)

### 2. Distribution of Sales
The target variable (Item Outlet Sales) is right-skewed, with most sales occurring at lower values and a few high-value outliers reaching up to 13,000.
<img width="1189" height="490" alt="download" src="https://github.com/user-attachments/assets/5c5aaa92-5304-4afd-a12f-8a6d7a018838" />


### 3. Sales Outliers by Outlet Type
Supermarket Type 3 stands out with significantly higher median sales and a larger range compared to Grocery Stores, which have the lowest performance.
<img width="868" height="639" alt="download" src="https://github.com/user-attachments/assets/d685da59-6c0d-42da-81f4-5751da70f531" />

### 4. Average Sales by Item Type (Type 3 Supermarkets)
In the most successful outlet type (Supermarket Type 3), "Breakfast" and "Fruits and Vegetables" are the top-performing categories.
<img width="1014" height="649" alt="download" src="https://github.com/user-attachments/assets/2a935e77-f9b9-4c30-9f4a-43957cf144bc" />

## Methods
- **Data Cleaning**: Handled missing values (imputation), corrected inconsistent categories (e.g., 'LF', 'low fat', 'Low Fat'), and checked for duplicates.
- **Feature Engineering**: Preprocessed the data using One-Hot Encoding for categorical variables and Scaling for numerical features through a Scikit-Learn Pipeline.
- **Machine Learning Modeling**: 
    - Linear Regression
    - Random Forest Regressor

## Results

#### Top Factors Influencing Sales
The analysis showed that the **Item_MRP** (Maximum Retail Price) has the strongest positive correlation with sales. 

#### Model Performance
The **Random Forest Model** performed significantly better than the Linear Regression model:
- **Test R²**: [0.604]
- **Test RMSE**: [1,044.663]

## Recommendations:
1. **Optimize Inventory for Type 3 Supermarkets**: Focus on high-performing categories like Breakfast and Produce.
2. **Pricing Strategy**: Leverage the strong correlation between MRP and Sales for revenue optimization.
3. **Outlet Expansion**: The Supermarket Type 3 model is the most profitable; consider mirroring its layout in other locations.

## For further information
For any additional questions, please contact **Hala Salah**.
