![image](https://github.com/user-attachments/assets/5dcacb17-14fc-4316-b307-2a1f754d2f1e)


# 📊 Product Sales Analysis Dashboard (Power BI)

This project is a Power BI report that provides clear insights into product performance, revenue generation, and category trends. It is designed to help stakeholders make data-driven decisions by visualizing key business metrics.

## 🔍 Project Overview

The dashboard answers key business questions such as:
- Which products generate the highest revenue?
- Which products are top sellers by volume?
- How is revenue distributed across categories?
- Which categories are the most popular?

## 🧮 Measures (DAX Calculations)

The following DAX measures were created to power the visualizations:

- **TotalUnitsSold**:
  ```dax
  TotalUnitsSold = SUM('TableName'[UnitsSold])
TotalRevenue:
TotalRevenue = SUMX('TableName', 'TableName'[UnitsSold] * 'TableName'[UnitPrice])
AvgRating:
AvgRating = AVERAGE('TableName'[Rating])
AvgPrice:
AvgPrice = AVERAGE('TableName'[UnitPrice])

📊 Visuals Included
Chart	Description	X-Axis	Y-Axis / Values
Revenue by Product Name	Compare total revenue per product	Product Name	TotalRevenue
Units Sold by Product Name	Identify top-selling products	Product Name	TotalUnitsSold
Revenue by Category	Show revenue distribution among categories	Category	TotalRevenue
Units Sold by Category	Highlight most popular categories	Category	TotalUnitsSold
🛠 Tools Used
Power BI Desktop

DAX (Data Analysis Expressions) for creating measures

Data Model with relationships between tables

Bar, Column, and Donut Charts for visualization

📁 How to Use
Clone or download this repository.

Open the .pbix file using Power BI Desktop.

Review and customize the data source if needed.

Explore the dashboard and interact with filters and visuals.

✨ Purpose
This project is meant to demonstrate:

Proficiency in Power BI and DAX

Data modeling and storytelling through visuals

Business insight delivery via dashboards

