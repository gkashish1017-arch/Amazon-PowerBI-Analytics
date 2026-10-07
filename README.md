# Amazon Product Analytics Dashboard | Power BI

An end-to-end **Amazon Product Analytics Dashboard** built using **Power BI, Power Query and DAX** to analyze product pricing, discounts, customer ratings, review engagement and category-level performance.

## 📌 Project Overview

This project analyzes an Amazon product-level dataset to identify meaningful patterns in:

* Product portfolio distribution
* Category performance
* Actual vs discounted pricing
* Discount strategies
* Customer ratings
* Customer review engagement
* Product-level performance
* Business opportunities and recommendations

The dashboard transforms raw product data into an interactive business intelligence solution designed for data-driven decision making.

## 🎯 Business Objective

The primary objective is to understand how Amazon's product portfolio varies across categories in terms of:

* Pricing
* Discounts
* Customer ratings
* Customer review engagement
* Availability of rating/review information

The analysis also provides actionable recommendations for pricing optimization, customer engagement and promotional strategy.

## 🛠️ Tools & Technologies

* **Power BI**
* **Power Query**
* **DAX**
* **Microsoft Excel / CSV**
* Data Cleaning & Transformation
* Data Visualization
* KPI Development
* Business Intelligence

## 📊 Dataset

**Source:** Kaggle Amazon Product Dataset

The dataset contains approximately:

* **1,465 product records**
* **1,351 unique products**

### Important Dataset Note

This is a **product-level dataset**, not a transaction-level sales dataset.

Therefore, the analysis intentionally avoids unsupported metrics such as:

* Revenue
* Profit
* Number of Orders
* Average Order Value
* Sales Growth

Instead, the project focuses on metrics that can be reliably calculated from the available product-level data.

## 🧹 Data Preparation

Data preparation was performed using **Power Query**.

Key transformation steps included:

* Standardized actual price and discounted price
* Converted price fields into numeric data types
* Converted discount percentage into a numeric format
* Extracted the primary rating from the original rating field
* Handled missing rating/review information
* Split hierarchical category information into multiple levels
* Created `Discount_Amount`
* Created `Discount_Status`
* Validated data types and errors before loading the data into Power BI

### Discount Classification

| Discount Percentage | Discount Status |
| ------------------- | --------------- |
| ≥ 50%               | High Discount   |
| ≥ 20% and < 50%     | Medium Discount |
| < 20%               | Low Discount    |

## 📈 Dashboard Structure

The Power BI dashboard contains **5 analytical pages**.

### 1. Executive Overview

Provides a high-level summary of the Amazon product portfolio.

Key analysis:

* Total Products
* Average Rating
* Average Discount
* Average Actual Price
* Average Discounted Price
* Average Discount Amount
* Products with Ratings
* High Discount Products
* Products by Category
* Discount Status Distribution
* Rating Distribution
* Top Products by Review Count

### 2. Category & Pricing Analysis

Focuses on category-level pricing and discount behavior.

Key analysis:

* Actual vs Discounted Price by Category
* Average Discount by Category
* Products by Category
* Price vs Rating by Category
* Average Discount Amount by Category

### 3. Rating & Discount Analysis

Analyzes the relationship between customer ratings, reviews and discount strategies.

Key analysis:

* Product Distribution by Rating
* Rating vs Customer Review Count
* Average Rating by Discount Status
* Average Rating by Category
* Average Discount by Rating
* Products by Discount Status

### 4. Product & Category Deep Dive

Provides detailed product-level and category-level analysis.

Key analysis:

* Top Products by Customer Review Count
* Price vs Rating by Category
* Average Discount by Category
* Actual vs Discounted Price
* Top Products by Discount Percentage
* Customer Review Count by Category

### 5. Business Insights & Recommendations

Converts analytical findings into business actions.

Key areas:

* Discount optimization
* Customer engagement
* Category-level pricing
* Promotional opportunities
* Pricing efficiency
* Margin protection

## 🔑 Key KPIs

| KPI                      |   Value |
| ------------------------ | ------: |
| Total Products           |   1,351 |
| Average Rating           |    4.10 |
| Average Discount         |  47.69% |
| Average Actual Price     | ~₹5.44K |
| Average Discounted Price | ~₹3.13K |
| Average Discount Amount  | ~₹2.32K |
| Products with Ratings    |   1,349 |
| High Discount Products   |     608 |

## 💡 Key Business Insights

### 1. High Discount Strategy

**608 products** fall under the High Discount category, indicating that discounting is a major pricing strategy across the analyzed product portfolio.

**Business implication:**
High-discount products should be reviewed to balance customer attraction with pricing efficiency and margin protection.

### 2. Broad Review Coverage

**1,349 products** have available customer rating/review information, providing broad review coverage across the analyzed product portfolio.

**Business implication:**
Highly reviewed products can be used as trust signals in recommendations and promotional campaigns.

### 3. Significant Pricing Opportunity

The average actual price is approximately **₹5.44K**, while the average discounted price is approximately **₹3.13K**.

**Business implication:**
Category-level discount optimization can help balance customer attraction with profitability.

###4. Strong Overall Product Rating

The overall average product rating is 4.10, indicating generally positive customer satisfaction across the analyzed product portfolio.

Business implication:
Highly rated products can receive stronger visibility through recommendations and promotional campaigns.

🎯 Business Recommendations
01 — Optimize Discount Strategy

Review products with very high discounts and evaluate whether the discount is generating sufficient customer engagement.

Expected Impact: Better pricing efficiency and improved margin protection.

02 — Promote High-Engagement Products

Prioritize products with high customer review counts and strong ratings in recommendations, promotional campaigns and category highlights.

Expected Impact: Higher product visibility and stronger customer trust.

03 — Use Category-Level Pricing Decisions

Compare pricing, discount levels, ratings and customer engagement across categories before making pricing or promotional decisions.

Expected Impact: More targeted category strategies and better allocation of promotional efforts.

📷 Dashboard Screenshots
1. Executive Overview
<img width="960" height="535" alt="01_Amazon_Overview" src="https://github.com/user-attachments/assets/977aad6b-c9e8-4f45-af7e-d3627f1f48bd" />


2. Category & Pricing Analysis
<img width="952" height="537" alt="02_Category_Pricing" src="https://github.com/user-attachments/assets/50fb7be8-5398-4a95-bdef-83e20831bd56" />




3. Rating & Discount Analysis
<img width="952" height="535" alt="03_Rating_Discount" src="https://github.com/user-attachments/assets/4ec8c9a9-3bb0-45fa-a780-c89b50d3e985" />




4. Product & Category Deep Dive
<img width="952" height="537" alt="04_Product_Deep_Dive" src="https://github.com/user-attachments/assets/5726078e-62f0-4670-85a6-848e67cc341a" />




5. Business Insights & Recommendations
<img width="960" height="532" alt="05_Business_Insights" src="https://github.com/user-attachments/assets/63172bf7-e451-43c6-b0f2-249523224158" />


📁 Project Structure
Amazon-PowerBI-Analytics/
│
├── README.md
├── Amazon_Product_Analytics.pbix
│
└── Dashboard_Screenshots/
    ├── 01_Amazon_Overview.png
    ├── 02_Category_Pricing.png
    ├── 03_Rating_Discount.png
    ├── 04_Product_Deep_Dive.png
    └── 05_Business_Insights.png



▶️ How to Use
Download the .pbix file from this repository.
Open it using Microsoft Power BI Desktop.
Explore the five dashboard pages.
Use the available slicers to interact with the analysis.
⚠️ Disclaimer

This project is created for educational, portfolio and data analytics demonstration purposes.

The dataset represents product-level information and does not provide transaction-level sales data. Therefore, metrics such as revenue, profit, orders and sales growth have not been included because they cannot be reliably calculated from the available data.

👩‍💻 Skills Demonstrated

Power BI | Power Query | DAX | Data Cleaning | Data Transformation | KPI Development | Data Visualization | Interactive Dashboards | Business Analysis | Business Insights

⭐ Project Outcome

This project demonstrates an end-to-end analytics workflow:

Raw Data → Data Cleaning → Transformation → DAX → KPI Development → Visualization → Business Insights → Recommendations
