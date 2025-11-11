# 🧩 Customer Retention Analytics Dashboard

## 📌 Project Overview
This Power BI project focuses on **Customer Retention and Churn Analysis** using a real-world styled dataset.  
It aims to identify **customer loyalty trends**, **churn rate**, and **business performance** through an interactive dashboard.

The analysis provides key insights into **customer behavior**, **sales performance**, **order outcomes**, and **average product ratings**.  
This project demonstrates the ability to perform **data cleaning**, **data modeling**, and **dashboard development** in Power BI.

---

## 💼 Key Objectives
- Analyze customer **churn rate** and **retention patterns**
- Identify **top-performing products and brands**
- Visualize **year-wise sales trends**
- Evaluate **order outcomes and delivery performance**
- Measure **average product ratings** and satisfaction levels
- Provide insights to **enhance loyalty programs** and reduce churn

---

## ⚙️ Tools & Technologies
| Tool / Technology | Purpose |
|--------------------|----------|
| **Power BI** | Dashboard creation & DAX measures |
| **Microsoft Excel / CSV** | Data cleaning and preprocessing |
| **DAX (Data Analysis Expressions)** | Calculations and KPI generation |
| **Data Modeling** | Establishing relationships between entities |

---

## 📊 Dashboard Features
| Feature | Description |
|----------|-------------|
| 💰 **Total Revenue & Orders** | Displays total amount raised and customer base |
| 🚚 **Category-based Outcome** | Visualizes the share of delivered, cancelled, and shipped orders |
| 🔁 **Churn Rate by Loyalty Tier** | Highlights which loyalty segments need focus |
| 🧾 **Top 5 Products & Brands** | Identifies high-demand items driving sales |
| 📈 **Year-wise Sales Trend** | Tracks business growth across years |
| ⭐ **Average Rating by Category** | Evaluates product satisfaction across categories |

---

## 🧮 Key DAX Measures

```DAX
-- Total Revenue
Total Revenue = SUM(master_table[order_total])

-- Average Rating
Average Rating = AVERAGE(master_table[rating])

-- Churn Rate (%)
Churn Rate (%) =
DIVIDE(
    COUNTROWS(FILTER(master_table, master_table[Is Churned] = "Churned")),
    COUNTROWS(master_table)
)

-- Average Delivery Days
Average Delivery Days = AVERAGE(master_table[Delivery Days])
