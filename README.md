# 📊 Superstore Sales Analysis (Power BI Dashboard)

This project presents a comprehensive sales and profit analysis of a Superstore over a 2-year period. Using **Power BI** and **DAX**, I created an interactive dashboard that visualizes key performance metrics to drive business insights.

![Dashboard Screenshot](./assets/dashboard.png) 

---

## 📁 Dataset

- **File**: `SuperStore_Sales_Dataset.csv`
- **Duration**: 2 years (2019–2020)
- **Features**: Sales, Profit, Orders, Discounts, Customer Segment, Category, Region, Shipping Mode, Payment Mode

---

## 🎯 Objectives

- Analyze overall business performance
- Understand regional and segment-wise profit trends
- Visualize order fulfillment times and shipping modes
- Track monthly sales/profit trends
- Provide an interactive dashboard for strategic decision-making

---

## 🧰 Tools & Technologies

- **Power BI**
- **DAX (Data Analysis Expressions)**
- **Power Query Editor** for data cleaning and transformation

---

## 📌 Dashboard Features

| 📈 Visual | Description |
|----------|-------------|
| **KPI Cards** | Total Sales (2M), Profit (175K), Orders (22K), Avg. Ship Days (10) |
| **Line Charts** | Monthly Sales & Profit trend (2019 vs. 2020) |
| **Donut Charts** | Sales by Segment, Payment Mode, Region |
| **Bar Charts** | Sales by Category, Sub-Category, and Ship Mode |
| **Map Visual** | Sales and Profit distribution across U.S. States |
| **Slicers** | Filter by Region: Central, East, South, West |

---

## 📊 Key DAX Measures

```DAX
Total Sales = SUM(Superstore[Sales])
Total Profit = SUM(Superstore[Profit])
Order Count = COUNT(Superstore[Order ID])
Avg Shipping Days = AVERAGE(DATEDIFF(Superstore[Order Date], Superstore[Ship Date], DAY))
Profit Margin = DIVIDE([Total Profit], [Total Sales])
