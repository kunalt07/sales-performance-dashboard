# 📊 Business Intelligence Dashboard for Sales Performance Analysis

## 🧾 Project Overview
This Power BI dashboard analyzes sales performance and profitability using the **Sample Superstore dataset**. It offers deep insights into **sales trends, regional performance, product profitability, and customer behavior**, helping businesses make informed strategic and operational decisions.

The dashboard empowers management to track KPIs, visualize patterns, and identify growth opportunities across multiple business dimensions.

---

## 🗂️ Dataset Overview

### 📘 Data Source
- **File Name:** `Sample - Superstore.xls`
- **Source:** Superstore dataset (a commonly used sample data by Tableau/Power BI).
- **Format:** Excel (.xls)
- **Rows:** ~10,000 records
- **Time Period Covered:** 2014 – 2017
- **Data Type:** Retail transactional data

### 📋 Sheets and Structure
| Sheet Name | Description |
|-------------|-------------|
| **Orders** | Contains detailed sales transactions (Order ID, Product, Sales, Profit, Quantity, Discount, etc.) |
| **Returns** | Records returned orders and reasons |
| **People** | Contains regional manager assignments |

---

## 🧮 Key Columns in the Orders Table
| Column | Description |
|---------|-------------|
| **Order ID** | Unique identifier for each transaction |
| **Order Date / Ship Date** | Timeline of orders and shipping |
| **Customer Name / Segment** | Information on customer type and segment |
| **Region / State / City** | Geographical sales distribution |
| **Category / Sub-Category / Product Name** | Product classification |
| **Sales / Profit / Quantity / Discount** | Financial metrics and performance indicators |
| **Ship Mode** | Shipping method used for delivery |

---

## 🛠️ Tools & Technologies Used
- **Power BI** – Data visualization and dashboard development
- **Excel (Sample Superstore)** – Data source
- **Power Query Editor** – Data cleaning and transformation
- **DAX (Data Analysis Expressions)** – Calculations and KPIs
- **Python (optional)** – For advanced data preprocessing and exploration

---

## 💻 Data Preparation & Modeling
- Cleaned missing and inconsistent values in the dataset.
- Created **calculated columns** and **measures** in Power BI:
  - `Profit Margin = Profit / Sales`
  - `Sales Growth %` using DAX time intelligence
  - `Average Delivery Time = DATEDIFF(Order Date, Ship Date, DAY)`
- Built a **star schema** with `Orders` as the fact table and `People` and `Returns` as dimension tables.

---

## 📊 Dashboard Design and Features

*Note: The images below will display correctly if you place your screenshot files (`By Date.png`, `By Region.png`, `By Product.png`) inside a folder named `screenshots` in your repository.*

### 1️⃣ Sales Overview
- KPIs: Total Sales, Total Profit, Profit Margin %, Number of Orders
- Visuals: KPI Cards, Monthly Sales Trend, Profit by Category
- Filter Options: Year, Region, and Segment
- The dashboard is interactive, allowing users to filter down to a specific date for granular analysis, as seen in this view for **January 13, 2014**.

![Dashboard filtered by a specific date](./screenshots/By%20Date.png)

### 2️⃣ Regional Performance
- Map visualization of sales across regions and states
- Top and Bottom 5 States by Revenue
- Sales by Ship Mode and Delivery Performance
- The dashboard allows for deep dives into specific geographical areas. For example, filtering by the **Central** region provides a focused view of its sales trends and segment distribution.

![Dashboard filtered by the Central region](./screenshots/By%20Region.png)

### 3️⃣ Product Analysis
- Category and Subcategory Sales Breakdown
- Top 10 Products by Profit
- Discount vs. Profit Correlation Scatter Plot
- Users can analyze performance by product category. The view below shows the dashboard filtered for the **Furniture** category, revealing its sales patterns and regional contributions.

![Dashboard showing Furniture category analysis](./screenshots/By%20Product.png)

### 4️⃣ Customer Insights
- Sales by Customer Segment (Consumer, Corporate, Home Office)
- Loyalty Analysis: Repeat vs. New Customers
- Profitability by Segment and Region

---

## 📈 Key Metrics and KPIs
| KPI | Description |
|------|--------------|
| **Total Sales** | Overall revenue generated |
| **Total Profit** | Net profit after discounts |
| **Profit Margin %** | Profit-to-sales ratio |
| **Sales Growth %** | YoY comparison |
| **Average Delivery Days** | Mean delivery duration per order |

---

## 🚀 Insights and Findings
- **West Region** contributes the highest sales, while **South** shows maximum growth potential.
- **Technology** category yields the highest profit margins.
- Excessive discounts in **Furniture** reduce profitability.
- **Corporate** segment has the highest average order value.
- **Standard Class shipping** is the most common and cost-effective mode.

---

## 💡 Future Enhancements
- Add predictive forecasting using Power BI’s AI visuals.
- Enable data refresh via Power BI Service for real-time tracking.
- Integrate customer segmentation clustering using Python.
- Automate KPI reporting using Power Automate.

---

## 👤 Author
**Kunal Tigga**
<br>_MBA in Business Analytics | Power BI & Data Analytics Enthusiast_
<br>📍 Bengaluru, India
<br>🔗 **LinkedIn:** [linkedin.com/in/your-profile-url](https://www.linkedin.com/in/your-profile-url)
<br>📧 **Email:** [your.email@example.com](mailto:your.email@example.com)
