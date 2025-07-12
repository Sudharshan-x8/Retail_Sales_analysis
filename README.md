# 🛍️ Retail Sales Analysis – EDA, Regression & Time Series (Python + Power BI)

## 📌 Project Overview

This project analyzes e-commerce retail data to uncover sales trends, product performance, customer behavior, and revenue patterns using:
- 🐍 Python (Pandas, Matplotlib, Scikit-learn)
- 📊 Power BI Dashboard (offline mode)
- ⏱ Time Series smoothing and regression modeling

---

## 🧠 Key Insights

- Identified top-selling products and customers
- Smoothed daily revenue trend using 7-day moving average
- Built linear regression model to understand revenue drivers
- Created an interactive Power BI dashboard to summarize KPIs

---

## 🛠️ Tools & Tech Used

- Python: Pandas, Matplotlib, Seaborn, Scikit-learn  
- Power BI (offline mode, screenshot attached)  
- Dataset: `Online Retail II` (CSV format)

---

## 📈 Dashboard Preview

📌 **Smoothed 7-Day Revenue Trend + KPIs Dashboard**

![Dashboard Preview](<img width="1201" height="673" alt="sales_dash_1" src="https://github.com/user-attachments/assets/7d045b8f-bd04-4252-b416-ce51f71c45c6" />)

![Dashboard Preview](<img width="1276" height="714" alt="sales_dash_2" src="https://github.com/user-attachments/assets/f4c72132-3af4-4584-b221-a90c87a406c8" />)

---

## 🔗 Project Files

- 📄 **[Case Study PDF](https://drive.google.com/file/d/12YcW3OOsJ6lVVHwHuaoh0UJovJGwtbNz/view?usp=drivesdk)**  
- 🧠 **[Python Notebook / Script](https://drive.google.com/file/d/1I8VYmxHGxR9aQRHc11isnUzi7B75r7QM/view?usp=drivesdk)**  

---

## 🧮 Sample SQL Queries Used

```sql
-- Total Revenue
SELECT SUM(price * quantity) AS Total_Revenue FROM online_sales;

-- Top-Selling Products
SELECT description, SUM(price * quantity) AS Revenue
FROM online_sales
WHERE quantity > 0 AND price > 0
GROUP BY description
ORDER BY Revenue DESC;
