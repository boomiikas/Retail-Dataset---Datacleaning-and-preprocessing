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
- `preprocessing.ipynb` → Jupyter Notebook with data cleaning pipeline  

---

## 🚀 Next Steps
- Perform **Exploratory Data Analysis (EDA)**.  
- Apply **Machine Learning models** for customer segmentation, sales prediction, or recommendation systems.  

---

👩‍💻 **Author:** Boomika S
