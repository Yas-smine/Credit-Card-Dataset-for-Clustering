# 📌 Credit Card Customer Segmentation (Clustering) – README

## 🔍 Project Overview
This project aims to segment credit card customers based on their spending behavior and credit usage. Using the **Credit Card Dataset for Clustering** (Kaggle), we analyze approximately **9,000 customers** to identify meaningful groups that can support targeted marketing strategies.

---

## 📁 Dataset Description
The dataset contains the following key features:

- **CUST_ID**: Unique customer ID  
- **BALANCE_FREQUENCY**: Frequency of balance updates (0–1)  
- **PURCHASES**: Total purchase amount  
- **CASH_ADVANCE**: Total cash advance amount  
- **CREDIT_LIMIT**: Assigned credit limit  
- **PAYMENTS**: Total payments made  

---

## 🛠️ Steps Performed

### 1️⃣ Data Import & Exploration
- Loaded dataset  
- Viewed first rows, shape, info, and summary stats  
- Checked for missing and corrupted values  

### 2️⃣ Data Preparation
- Cleaned missing values  
- Removed outliers when necessary  
- Scaled numerical features using StandardScaler  
- Selected the two features required for clustering:
  - `PURCHASES`
  - `CREDIT_LIMIT`

---

## 3️⃣ Hierarchical Clustering
- Built dendrogram using `scipy.cluster.hierarchy`  
- Identified **3 natural clusters** from largest vertical linkage  
- Created scatter plot to visualize hierarchical clusters  

---

## 4️⃣ K-Means Clustering
- Tested several values of k  
- Applied the **Elbow Method**  
- Optimal number of clusters: **k = 3**  
- Trained final K-Means model and plotted clusters  

---

## 📊 Cluster Interpretation

### **Cluster 1 – High-Value Customers**
- High purchases  
- High credit limit  
- Represents premium customers with strong spending ability  

### **Cluster 2 – Medium Customers**
- Moderate credit limit  
- Low to medium purchases  
- Customers with potential for targeted promotions  

### **Cluster 3 – Low-Value Customers**
- Low purchases  
- Low credit limit  
- Lower activity; require basic services or close monitoring  

---

## 🧠 Business Insights
- Premium customers should receive **loyalty programs and exclusive offers**  
- Medium customers can be encouraged with **marketing campaigns**  
- Low-value customers may need **risk evaluation or basic credit services**  

---

## 🚀 Technologies Used
- **Python**, **Pandas**, **NumPy**  
- **Matplotlib**, **Seaborn**  
- **SciPy** for hierarchical clustering  
- **Scikit-Learn** for K-Means and scaling  


