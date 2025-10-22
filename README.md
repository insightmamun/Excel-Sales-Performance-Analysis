# Sales Performance Analysis – Excel Dashboard Project

## Project Overview
This project demonstrates a complete Excel data analysis workflow to evaluate and visualize the sales performance of a gift item delivery company. The dashboard provides key insights on total revenue, order volume, average delivery time and customer spending patterns across various occasions, products, and cities. The analysis helps identify sales trends, seasonal peaks, and operational efficiency opportunities.

---

## Objective
The objective is to transform raw transactional data into a clean, insightful, and interactive Excel dashboard using **Power Query** and **Power Pivot**.  

---

## Tools
- **Microsoft Excel**
- **Power Query** – for data cleaning and transformation  
- **Power Pivot / Data Model** – for building relationships and DAX-based measures  
- **PivotTables & PivotCharts** – for interactive visualization  
- **Slicers & Timeline Filters** – for user-driven interactivity and exploration

---

## Data Sources
Data includes:
- **Orders Table:** order_id, customer_id, product_id, quantity, order_date, order_time, , delivery_date, delivery_time, location, occasion 
- **Products Table:** product_id, product_name, category, price, occasion  
- **Customer Table:** customer_id, name, city, contact_no, email, gender, address  

Relationships were created in a **star schema** model with the Orders table as the fact table and other tables as dimensions.

---

## Data Preparation
1. Imported raw Excel files into Power Query.  
2. Cleaned and standardized fields (trim, case fix, null removal).  
3. Derived new columns: month_name, difference_of_order_delivery_day, delivery_time_hour
4. Loaded cleaned data into the Power Pivot Data Model.

---

## Data Modeling
- Created relationships between Order, Products, and Customer tables.  
- Defined core **DAX measures**:
  - `Total Revenue = Orders[price]*Orders[Quantity]`
  - `Total Orders = DISTINCTCOUNT(Orders[order_id])`
- Established a reusable model for future reporting.

---

## Dashboard Design
The Excel dashboard consists of interactive PivotCharts and slicers presenting key business metrics.

**Key Performance Indicators**
- Total Revenue: £89,353.50  
- Total Orders: 900  
- Average Delivery Time: 1.98 days  
- Average Spending: £99.28  

**Visual Sections**
- Monthly Revenue Trend  
- Revenues by Occasion (Anniversary, Christmas, Valentine’s Day, etc.)  
- Most Ordering Time (by hour)  
- Top 10 Products by Revenue  
- Top 5 Product Categories  
- Top 10 Cities by Order Volume  
- Interactive filters for Occasion and Date Range  

---

## Insights and Findings
- **Seasonal Trends:** Highest revenues occur during **Anniversary** and **Christmas** periods.  
- **Top Categories:** **Hampers** and **Perfumes** lead total revenue.  
- **Peak Order Hours:** Customer orders peak around **evening hours (17–18h)**.  
- **Geographic Insights:** **Leeds**, **Bristol**, and **Birmingham** show the highest order counts.  
- **Operational Insight:** Average delivery time of ~2 days aligns with fulfillment standards.

---

## Skills Demonstrated

Data cleaning, Power Query, Power Pivot, DAX calculations, dashboard design, KPI creation, data storytelling, trend analysis, and Excel automation, Insight generation, performance evaluation,


---

## Summary
This Excel project showcases the ability to:
- Transform and model raw data into a structured schema.  
- Design clean and interactive dashboards with real insights.  
- Communicate data-driven decisions effectively using Excel’s advanced analytics capabilities.

---

## Dashboard Preview
<img width="1852" height="788" alt="Image" src="https://github.com/user-attachments/assets/f4ee67f8-7dd2-4a2f-a578-a44916bcf79b" />

---
