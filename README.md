# 🛒 Retail Dataset – Data Cleaning & Preprocessing

## 📌 Project Overview
This project focuses on **data inspection, cleaning, and preprocessing** of a retail dataset.  
The dataset contains **2000 customer transactions** with 11 columns.  

The goal is to prepare a **cleaned dataset (`Retail_Cleaned.csv`)** for further analysis and modeling.

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

## 🔍 Data Inspection
- Checked dataset size, structure, and column details.  
- Verified data types for each column.  
- Identified missing values, duplicates, and inconsistencies.  

---

## 🧹 Data Cleaning Steps
1. **Missing Data Handling**
   - Replaced missing **Age** with median.  
   - Replaced missing **City** with most frequent value.  
   - Dropped rows with missing **TransactionID** or **ProductCategory**.  

2. **Data Cleaning**
   - Removed duplicate transactions.  
   - Standardized categorical values (e.g., `m, Male, MALE → Male`).  
   - Removed invalid entries (negative/zero `Quantity` or `Price`).  

---

## 🏗️ Feature Engineering
- **TotalAmount** derived if missing (`Quantity × Price`).  
- Extracted **Month** and **DayOfWeek** from `PurchaseDate`.  
- Created **AgeGroup** categories:  
  - 18–25, 26–40, 41–60, 60+  

---

## 🔠 Encoding & Transformation
- Encoded categorical columns (`Gender`, `City`, `ProductCategory`).  
- Normalized numeric columns (`Age`, `Price`, `TotalAmount`) using **MinMaxScaler**.  

---

## ✅ Final Verification
- No missing or invalid values remain.  
- Cleaned dataset saved as **`Retail_Cleaned.csv`**.  

---

## 📂 Files
- `Retail.csv` → Raw dataset  
- `Retail_Cleaned.csv` → Cleaned dataset  
- `tcs ds.ipynb` → Jupyter Notebook with data cleaning pipeline  

---

# 📊 Exploratory Data Analysis (EDA)

To better understand the dataset, various **visualizations** were created using Matplotlib and Seaborn.

---

### 1. Age Distribution
- **Histogram** shows the distribution of customers by age.
  
<img width="571" height="432" alt="image" src="https://github.com/user-attachments/assets/ea8fd6d7-0a16-4952-ae1c-a16594d2f673" />

- **KDE Plot** (Kernel Density Estimation) provides a smooth curve of age distribution.
  <img width="567" height="432" alt="image" src="https://github.com/user-attachments/assets/03795f6a-a4cc-4fb0-8fd9-23ac684197e5" />
  
---

### 2. Gender Distribution
- **Bar chart** showing counts of Male/Female customers.
  <img width="571" height="453" alt="image" src="https://github.com/user-attachments/assets/40b9f383-1ebd-4172-89f2-cb448a353885" />

---

### 3. Top 10 Cities by Customers
- Bar chart of the **most frequent cities** with the highest number of customers.
  <img width="571" height="523" alt="image" src="https://github.com/user-attachments/assets/2a3ed703-5f14-4520-bed3-0743f0b59902" />


---

### 4. Product Category Revenue
- Bar chart of **total revenue contribution by product categories**.
  <img width="543" height="494" alt="image" src="https://github.com/user-attachments/assets/050d68e1-031a-4d7c-a0c2-b45fa1f3dfae" />


---

### 5. Monthly Sales Trend
- Line chart showing **sales trend across months**.
  <img width="563" height="453" alt="image" src="https://github.com/user-attachments/assets/00f8f03e-bea6-4337-b360-98996471d84e" />


---

### 6. Payment Mode Distribution
- **Pie chart** showing percentage distribution across payment modes.
  <img width="515" height="409" alt="image" src="https://github.com/user-attachments/assets/2c7458f8-4649-4324-8f6b-7aeddbf2e4c9" />

---

### 7. Average Spend by Age Group
- Bar chart showing **average spend per customer** across age groups.
  <img width="576" height="479" alt="image" src="https://github.com/user-attachments/assets/f0d8911c-0064-44b1-ae3a-9476a81eb08e" />


---

### 8. Top 10 Cities by Revenue Contribution
- Bar chart of cities contributing the most to total revenue.

---

### 9. Product Category vs Payment Mode
- **Heatmap** showing the relationship between product categories and payment modes.
<img width="592" height="453" alt="image" src="https://github.com/user-attachments/assets/e4803676-492c-45dc-83d3-1ba0001c6e65" />


---

## 🚀 Next Steps 
- Apply **Machine Learning models** for customer segmentation, sales prediction, or recommendation systems.  

---

👩‍💻 **Author:** Boomika S
