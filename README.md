# Flipkart Business Analytics Dashboard

An interactive **Flipkart Business Analytics Dashboard** developed using **Microsoft Power BI** and **DAX** to analyze sales, products, categories, sellers, customers, and business operations.

---

## 📌 Project Overview

This project presents a 5-page interactive Power BI dashboard designed to analyze Flipkart business data and provide meaningful insights into overall business performance.

The dashboard includes analysis of:

- Sales and Revenue
- Products and Categories
- Sellers and Locations
- Customers and Reviews
- Delivery and Stock
- Returns and Operations

Interactive filters and visualizations allow users to explore the data from different perspectives.

---

# 📑 Dashboard Pages

## 🏠 1. Executive Overview

The Executive Overview provides a high-level summary of the overall business performance.

### Key KPIs
- Total Products: **80K**
- Total Units Sold: **201M**
- Total Revenue: **4.76T**
- Average Selling Price: **23.70K**
- Average Discount: **21.35**
- Average Rating: **3.00**

### Visualizations
- Revenue by Category
- Units Sold by Year
- Revenue by Brand
- Revenue by Seller City
- Interactive filters for Year, Brand, Category, Seller, and Seller City

---

## 💰 2. Sales & Revenue Analysis

This page focuses on sales performance, revenue trends, pricing, and discount analysis.

### Key KPIs
- Total Revenue: **4.76T**
- Total Units Sold: **201M**
- Average Selling Price: **23.70K**
- Average Discount: **21.35**
- Total Products: **80K**

### Visualizations
- Discount Percentage vs Units Sold
- Revenue by Year-Month
- Units Sold vs Revenue by Category
- Revenue by Category
- Interactive filters for Year, Brand, Category, Seller, and Seller City

---

## 📦 3. Product & Category Analysis

This page provides detailed insights into product and category performance.

### Key KPIs
- Total Products: **80K**
- Total Units Sold: **201M**
- Average Selling Price: **23.70K**
- Average Product Score: **50.67**
- Total Reviews: **2B**

### Visualizations
- Revenue by Category
- Top Products by Revenue
- Units Sold by Category
- Products by Rating
- Revenue by Brand
- Product Score and Review Count by Rating

---

## 👤 4. Seller & Location Analysis

This page analyzes seller performance and geographical distribution.

### Key KPIs
- Total Cities: **8**
- Total Sellers: **8**
- Total Revenue: **4.76T**
- Average Seller Rating: **4.00**

### Visualizations
- Seller Rating Gauge
- Revenue by Seller
- Revenue by Category and Seller
- City-wise Seller Analysis
- Category-wise Seller Revenue Matrix
- Seller and Location comparison

### Cities Analyzed
- Ahmedabad
- Bengaluru
- Chennai
- Delhi
- Hyderabad
- Kolkata
- Mumbai
- Pune

---

## ⭐ 5. Customer & Operations Analysis

This page focuses on customer engagement and operational performance.

### Key KPIs
- Total Stock: **40M**
- Average Delivery Days: **6.01**
- Returnable Products: **80K**

### Visualizations
- Review Count by Rating
- Stock vs Units Sold by Category
- Products by Delivery Days
- Revenue Contribution by Category
- Customer and operational performance analysis

---

# 🛠️ Tools & Technologies

- **Microsoft Power BI**
- **DAX (Data Analysis Expressions)**
- **Power Query**
- **Data Visualization**
- **Business Intelligence**
- **CSV Dataset**

---

# 📊 Key DAX Measures

The dashboard uses several DAX measures for business analysis, including:

Total Products =
DISTINCTCOUNT('flipkard'[product_id])

Total Units Sold =
SUM('flipkard'[units_sold])

Total Revenue =
SUMX(
    'flipkard',
    'flipkard'[final_price] * 'flipkard'[units_sold]
)
Average Selling Price =
AVERAGE('flipkard'[final_price])
Average Discount =
AVERAGE('flipkard'[discount_percent])
Average Rating =
AVERAGE('flipkard'[rating])
Total Stock =
SUM('flipkard'[stock_available])
Average Seller Rating =
AVERAGE('flipkard'[seller_rating])
Total Reviews =
SUM('flipkard'[review_count])








