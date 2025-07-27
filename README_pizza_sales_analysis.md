
# 📊 Pizza Sales Analysis Dashboard

An end-to-end data analytics project focused on analyzing pizza sales data using **SQL** and **Power BI**. The goal is to uncover actionable insights around revenue, ordering trends, and customer behavior to support business decision-making.

---

## 🧾 Project Summary

This project analyzes a pizza restaurant’s sales data to identify key metrics and trends including:
- Total revenue
- Average order value
- Best-selling pizzas
- Daily and hourly order patterns
- Category and size-wise sales performance

---

## 🛠️ Tools & Technologies

- **SQL (MySQL)** – Data wrangling, aggregation & KPI generation
- **Power BI** – Interactive dashboard and data visualization
- **Excel/CSV** – Source data file handling

---

## 📁 Project Files

| File Name                          | Description                                      |
|-----------------------------------|--------------------------------------------------|
| `Pizza_Sales.csv`                 | Raw dataset containing order-level details       |
| `Pizza Sales Analysis Queries.sql`| SQL queries used for data analysis               |
| `Pizza Sales Analysis Dashboard.pbix` | Power BI report visualizing key metrics     |

---

## 📌 Key Insights

- **Friday** saw the highest number of orders.
- **Regular-size pizzas** generated the highest revenue share.
- Top 5 pizzas accounted for a major portion of total sales.
- Most orders were placed around **noon and evening hours**.

---

## 📈 Sample SQL Queries

```sql
-- Total Revenue
SELECT ROUND(SUM(total_price), 2) AS total_revenue FROM pizza_sales;

-- Best Sellers
SELECT pizza_name, SUM(quantity) AS Total_Pizza_Sold
FROM pizza_sales
GROUP BY pizza_name
ORDER BY Total_Pizza_Sold DESC
LIMIT 5;
```

---

## 🧠 Learning Outcomes

- Applied SQL for real-world business metric computation
- Created an end-to-end BI dashboard in Power BI
- Developed storytelling through data visuals

---

## 🚀 How to Use

1. Clone the repository or download files
2. Open `Pizza Sales Analysis Dashboard.pbix` in Power BI Desktop
3. Open `Pizza Sales Analysis Queries.sql` in a SQL client
4. Load and explore `Pizza_Sales.csv` to try your own queries
