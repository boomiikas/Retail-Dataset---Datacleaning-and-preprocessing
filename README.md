# 🛒 Retail Dataset – Data Cleaning, Preprocessing & EDA  

## 📌 Project Overview  
This project focuses on **data inspection, cleaning, preprocessing, and exploratory data analysis (EDA)** of a retail dataset.  
The dataset contains **2000 customer transactions** with 11 columns.  

The goal is to prepare a **cleaned dataset (`Retail_Cleaned.csv`)** and generate **insights through EDA** for further modeling.  

---

## 📊 Dataset Information  
**Shape:** 2000 rows × 11 columns  

| Column Name      | Description |
|------------------|-------------|
| TransactionID    | Unique ID for each transaction |
| CustomerID       | Unique ID for each customer |
| Gender           | Customer gender (Male/Female) |
| Age              | Customer age (integer) |
| City             | Customer city |
| ProductCategory  | Purchased product category |
| Quantity         | Quantity of product purchased |
| Price            | Price per unit |
| PurchaseDate     | Date of purchase |
| PaymentMode      | Payment method (Cash/Card/UPI/etc.) |
| TotalAmount      | Total transaction amount (Quantity × Price) |

---

# 📊 Exploratory Data Analysis (EDA)  

To **visualize and understand patterns**, several plots were generated using **Matplotlib & Seaborn**.  

✨ *This section highlights the most engaging part of the project!*  

---

### 1. Age Distribution  
- Histogram + KDE curve show the spread of customers’ ages.  
<img width="571" height="432" src="https://github.com/user-attachments/assets/ea8fd6d7-0a16-4952-ae1c-a16594d2f673" />  
<img width="567" height="432" src="https://github.com/user-attachments/assets/03795f6a-a4cc-4fb0-8fd9-23ac684197e5" />  

---

### 2. Gender Distribution  
- Bar chart showing counts of Male vs Female customers.  
<img width="571" height="453" src="https://github.com/user-attachments/assets/40b9f383-1ebd-4172-89f2-cb448a353885" />  

---

### 3. Top 10 Cities by Customers  
- Which cities have the highest customer base?  
<img width="571" height="523" src="https://github.com/user-attachments/assets/2a3ed703-5f14-4520-bed3-0743f0b59902" />  

---

### 4. Product Category Revenue  
- Total revenue contribution by product categories.  
<img width="543" height="494" src="https://github.com/user-attachments/assets/050d68e1-031a-4d7c-a0c2-b45fa1f3dfae" />  

---

### 5. Monthly Sales Trend  
- Line chart showing seasonal or monthly purchase patterns.  
<img width="563" height="453" src="https://github.com/user-attachments/assets/00f8f03e-bea6-4337-b360-98996471d84e" />  

---

### 6. Payment Mode Distribution  
- Pie chart of customer payment preferences.  
<img width="515" height="409" src="https://github.com/user-attachments/assets/2c7458f8-4649-4324-8f6b-7aeddbf2e4c9" />  

---

### 7. Average Spend by Age Group  
- Which age groups spend the most?  
<img width="576" height="479" src="https://github.com/user-attachments/assets/f0d8911c-0064-44b1-ae3a-9476a81eb08e" />  

---

### 8. Top 10 Cities by Revenue Contribution  
- Cities contributing the most to sales revenue.  

---

### 9. Product Category vs Payment Mode  
- Heatmap showing the relationship between categories & payment modes.  
<img width="592" height="453" src="https://github.com/user-attachments/assets/e4803676-492c-45dc-83d3-1ba0001c6e65" />  

---

# 🧹 Data Cleaning & Preprocessing  

### 🔍 Data Inspection  
- Verified dataset shape, data types, and column info.  
- Checked for missing values, duplicates, and invalid entries.  

### 🛠️ Steps Performed  
1. **Missing Data**  
   - Filled `Age` with median, `City` with mode.  
   - Dropped rows with missing `TransactionID` / `ProductCategory`.  

2. **Data Cleaning**  
   - Removed duplicates.  
   - Standardized categorical values (e.g., `m, MALE → Male`).  
   - Removed invalid `Quantity` or `Price` entries.  

3. **Feature Engineering**  
   - Derived `TotalAmount` where missing.  
   - Extracted `Month` & `DayOfWeek` from `PurchaseDate`.  
   - Created `AgeGroup` buckets: 18–25, 26–40, 41–60, 60+.  

4. **Encoding & Scaling**  
   - Encoded categorical features.  
   - Normalized numeric features using MinMaxScaler.  

✅ Final dataset saved as **`Retail_Cleaned.csv`**.  

---

## 📂 Files  
- `Retail.csv` → Raw dataset  
- `Retail_Cleaned.csv` → Cleaned dataset  
- `tcs ds.ipynb` → Notebook with full pipeline  

---

## 🚀 Next Steps  
- Apply **ML models** for segmentation, prediction, or recommendation.  

---

👩‍💻 **Author:** Boomika S  
