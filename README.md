# 🛒 ShopSphere Online – E-Commerce Business Analytics Dashboard

An interactive **Power BI Business Analytics Dashboard** built using the **Brazilian E-Commerce (Olist) dataset** to analyze revenue, sales trends, product performance, customer behavior, delivery performance, and regional purchasing patterns.

---

## 📌 Project Overview

**ShopSphere Online** is an e-commerce business analytics project designed to transform raw e-commerce data into meaningful business insights.

The dashboard helps answer important business questions such as:

* How much revenue was generated?
* Which product categories generate the most revenue?
* Which customers contribute the most revenue?
* How do sales change month by month?
* Which categories have high or low customer ratings?
* Which regions contribute the most sales?
* Which products and categories are frequently purchased?
* Which categories require attention?
* What factors influence customer satisfaction?
* What actions can the business take based on the data?

---

## 🎯 Objectives

The main objectives of this project are to:

* Analyze overall e-commerce sales performance
* Identify high-performing product categories
* Understand customer purchasing behavior
* Analyze regional sales patterns
* Study customer review ratings
* Analyze delivery performance
* Identify underperforming categories
* Track monthly revenue trends
* Create actionable business recommendations

---

## 📊 Dataset

The project uses the **Brazilian E-Commerce Public Dataset by Olist**.

The dataset contains approximately:

* **96K orders**
* **96K customers**
* **71 product categories**
* **13.59M total revenue**

The project uses **9 source tables**, including:

* Orders
* Order Items
* Payments
* Reviews
* Customers
* Products
* Sellers
* Geolocation
* Product Category Translation

---

## 🛠️ Tools & Technologies

| Tool / Technology      | Purpose                                 |
| ---------------------- | --------------------------------------- |
| **Microsoft Power BI** | Dashboard development and visualization |
| **Power Query**        | Data cleaning and transformation        |
| **DAX**                | Business calculations and KPIs          |
| **CSV Dataset**        | Raw data source                         |
| **Star Schema**        | Data modeling                           |

---

## 🔄 Data Preparation

The raw dataset was prepared using Power Query before creating the dashboard.

### Main preprocessing steps

1. Imported all 9 CSV tables into Power BI
2. Corrected date and time data types
3. Translated Portuguese product categories into English
4. Reduced duplicate geolocation records
5. Removed duplicate reviews
6. Cleaned city and state names
7. Prepared the data for analysis and visualization

---

## 🏗️ Data Modeling

The project uses a **Star Schema** for the Power BI data model.

**Order Items** acts as the central fact table, while supporting tables provide information about customers, orders, products, sellers, payments, reviews, geolocation, and dates.

This model allows filters and slicers to interact across the dashboard efficiently.

---

## 🧮 Key DAX Measures

Some of the important measures created for the dashboard include:

### Total Revenue

```DAX
Total Revenue = SUM(Order_items[price])
```

### Order Count

```DAX
Order Count = DISTINCTCOUNT(Orders[order_id])
```

### Average Order Value

```text
Average Order Value = Total Revenue / Order Count
```

### Average Review Score

```DAX
Avg Review Score = AVERAGE(Order_reviews[review_score])
```

Other measures include:

* Late Delivery %
* Average Days Early/Late
* Month-over-Month Revenue Growth %
* Repeat Customer %

---

## 📈 Dashboard Pages

### 1️⃣ Overview

The Overview page provides an executive summary of the business.

It includes:

* Total Revenue
* Total Orders
* Average Order Value
* Customer Count
* Monthly Revenue Trend
* Payment Method Breakdown
* Revenue by State

### 2️⃣ Products & Categories

This page focuses on product and category performance.

It includes:

* Top Revenue-Generating Categories
* Revenue Treemap
* Revenue vs Review Score Analysis
* Category Performance Table

### 3️⃣ Customers & Regions

This page focuses on customer and regional behavior.

It includes:

* Top Customers by Revenue
* Delivery Performance vs Review Score
* Payment Installment Analysis
* Regional Purchasing Patterns

---

## 🔍 Key Insights

### 💰 Revenue Performance

The dashboard recorded approximately **13.59M in total revenue from 96K orders**, with an average order value of approximately **140.90**.

### 🛍️ Top Categories

The leading revenue-generating categories include:

* Health & Beauty
* Watches & Gifts
* Bed & Bath Table

### 📅 Monthly Sales Trend

Revenue remains relatively steady across most months, with a noticeable decline in **September** that requires further investigation.

### 🚚 Delivery Performance

Orders were delivered approximately **13 days ahead of the estimated delivery date on average**, with the analysis showing a relationship between delivery performance and customer review scores.

### 📍 Regional Performance

A significant share of revenue comes from the **Southeast region of Brazil**, particularly around São Paulo.

### ⚠️ Underperforming Categories

The revenue-versus-rating analysis helps identify categories with both **lower revenue and lower customer ratings**, highlighting areas that may require further investigation.

---

## 💡 Business Recommendations

Based on the dashboard analysis, the project provides five major recommendations:

1. **Focus on high-performing categories**
   Increase inventory and promotional activities for the strongest revenue-generating categories.

2. **Investigate the September sales decline**
   Analyze stock levels, marketing activities, and seller performance to identify the possible cause.

3. **Maintain strong delivery performance**
   Continue monitoring logistics and delivery service levels.

4. **Review underperforming categories**
   Investigate pricing, seller quality, product information, and customer feedback.

5. **Strengthen regional strategies**
   Maintain the existing strong presence in the Southeast while exploring opportunities in other regions.

---

## 📌 Project Highlights

* ✅ 9 raw data tables cleaned and integrated
* ✅ Star-schema data model
* ✅ Multiple DAX measures
* ✅ 3 interactive Power BI dashboard pages
* ✅ 10 business questions addressed
* ✅ Data-driven business insights
* ✅ Actionable recommendations

---

---

## 🎓 Project Information

**Project:** E-Commerce Business Analytics Dashboard – ShopSphere Online
**Role:** Data Analyst
**Tool:** Microsoft Power BI
**Dataset:** Brazilian E-Commerce (Olist)
**Developer:** Prakruthi B R

---

## 🚀 Skills Demonstrated

**Power BI • Power Query • DAX • Data Cleaning • Data Modeling • Data Visualization • Business Analytics • KPI Analysis • Customer Analytics • E-Commerce Analytics • Business Intelligence**

---

## 📬 Conclusion

This project demonstrates how raw e-commerce data can be transformed into an interactive business intelligence solution.

The ShopSphere dashboard brings together **revenue, products, customers, delivery performance, and regional data** in one place, helping businesses identify trends, understand performance, and make data-driven decisions.

