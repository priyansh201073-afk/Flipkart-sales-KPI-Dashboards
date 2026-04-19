# Flipkart Sales KPI Dashboard

This is a Power BI dashboard I built using a Flipkart e-commerce dataset as part of my Data Analyst preparation. The goal was to go beyond basic drag-and-drop visuals and actually write DAX measures from scratch to answer real business questions.

---


---

## Why I Built This

I wanted to practice building something that reflects what a DA/BA actually does — take raw sales data, model it properly, write meaningful measures, and present insights in a clean, decision-ready format. This dashboard is the result of that.

---

## Tools Used

- Power BI Desktop
- DAX — for all custom measures
- Power Query — for data cleaning
- Star Schema — for the data model

---

## What the Dashboard Shows

- Total revenue, orders, average customer rating, and average discount
- Which product categories generate the most sales
- Month-over-month sales growth trend across the year
- Regional sales ranking using RANKX
- Payment method breakdown (UPI, COD, Debit Card)

---

## DAX Measures I Wrote

| Measure | Purpose |
|---|---|
| Total Sales | Sum of all order revenue |
| Total Orders | Count of all orders |
| Average Customer Rating | Overall satisfaction score |
| Avg Discount % | Average discount across orders |
| MoM Growth % | Month-over-month sales growth using DATEADD |
| Sales YTD | Year-to-date cumulative sales using TOTALYTD |
| Sales MTD | Month-to-date sales using TOTALMTD |
| Last Year Sales | Year-over-year comparison using SAMEPERIODLASTYEAR |
| % of Total Sales | Each category's contribution using DIVIDE + ALL |
| Region Rank | Regional ranking by sales using RANKX + CALCULATE |

---

## Data Model

I built a star schema with a fact table (sales transactions) connected to a dedicated Date dimension table — which is required for Time Intelligence functions like TOTALYTD and SAMEPERIODLASTYEAR to work correctly.

---

## A Few Findings

- South region has the highest sales among all 5 regions
- Grocery is the best performing product category
- UPI is the most used payment method
- Average discount being offered is around 14.45%

---

## About Me

I'm Priyansh, a PGDM graduate in Operations & Business Analytics, currently building my skills in SQL, Power BI, and DAX to transition into a Business/Data Analyst role.

[LinkedIn](https://www.linkedin.com/in/priyanshukumar-analyst) • [GitHub](https://github.com/priyansh201073-afk)
