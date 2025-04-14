# 🛒 Online Retail

## 📌 Project Overview

This project delivers a complete **Exploratory Data Analysis (EDA)** of a real-world e-commerce dataset. It focuses on identifying actionable insights related to **sales performance**, **customer behavior**, and **product returns**, offering a data-driven foundation for strategic business decisions.

The dataset contains transactional data from an online retail store, with details like invoice numbers, product descriptions, quantities, prices, customer IDs, and countries of purchase.

---

## 📁 Project Structure

- `source/` – Raw dataset.
- `online_retail.ipynb` – Full EDA notebook.
- `README.md` – Project overview and conclusions.
- `requirements.txt` – Required libraries.

---

## 🧹 Data Preparation

Before analysis, several preprocessing steps were applied:
- Handled missing values in `CustomerID` and `Description`.
- Converted columns to appropriate data types.
- Removed duplicates and inconsistent values.
- Addressed invalid or negative entries in `Quantity` and `UnitPrice`.
- Classified transactions as **Sale**, **Return**, or **Special Case** based on invoice patterns and quantity signs.

---

## 📊 Key Sections

### 1. **Sales Performance Overview**
- The **United Kingdom** dominates in both revenue and volume.
- The product **REGENCY CAKESTAND 3 TIER** generated the most revenue; **PAPER CRAFT, LITTLE BIRDIE** had the highest sales volume.
- **Average Order Value (AOV)**: \$478.26
- A small number of high-value customers are responsible for a large portion of revenue, highlighting opportunities for retention strategies.

### 2. **Customer Behavior and RFM Analysis**
- Customers were segmented using **Recency**, **Frequency**, and **Monetary** (RFM) metrics.
- High RFM scores revealed loyal and valuable customers for personalized engagement.
- Behavioral patterns were visualized through RFM segmentation and distribution plots.

### 3. **Product Return Analysis**
- Return rate per country was calculated **as a proportion of total sales**, allowing fair comparisons across different sales volumes.
- The **UK**, while having the highest return volume, showed a return rate of **~9.3%**, which is moderate given its sales size.
- Several top-selling products like **PAPER CRAFT, LITTLE BIRDIE** and **MEDIUM CERAMIC TOP STORAGE JAR** had **return rates exceeding 90%**, indicating potential product issues or misalignment with customer expectations.

---

## 🧠 Insights & Recommendations

- **Customer segmentation** offers a strong foundation for targeted marketing and improving customer lifetime value.
- **Return-prone products** should be reviewed for quality assurance or better product communication.
- The business should consider **return rate reduction strategies** to improve margins without compromising sales.
- High-performing countries like the UK remain crucial, while others such as the **Netherlands**, **Eire**, and **Germany** offer growth potential with relatively low return rates.

---

## 🧰 Technologies Used

- **Python**
- **Pandas, NumPy** – Data manipulation
- **Matplotlib, Seaborn** – Visualization
- **Jupyter Notebook** – Analysis environment

---

## ▶️ How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/online-retail-analysis.git
   cd online-retail-analysis
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Launch the notebook:
   ```bash
   jupyter notebook
   ```