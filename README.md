# Coffee Bean Orders Analysis (Product, Loyalty, and Seasonal Trends Analysis)

## Table of Contents
1. Project Overview
2. Business Problem 
3. Data Sources
4. Data Cleaning and Transformation (Power Query)
5. Data Modelling
6. DAX Measures Created
7. Dasboard Design & Visuals
   - Page 1: Overview Dashboard
   - Page 2: Salesperson-details
8. Key Insights from the Dashboard
9. Tools Used
10. Project Delieverables 
11. Potential Extensions


   ---
   ## 1. Project Overview
   This Project demonstrates end-to-end Coffee Bean Shop data collection, followed by data cleaning in **Power Query**, and finally performing explorative analysis and visualization in **Power Bi.**
   Interactive Power BI dashboard analyzing coffee bean sales to identify top-performing products, geographic revenue drivers, loyalty program effectiveness, and seasonal revenue fluctuations. Supports inventory decisions, marketing targeting, and retention strategies for a coffee retailer. 
   This dashboard support data-driven decision-making by summarizing coffee sales trends and highlighting areas that needs managerial attention.

---
## 2. Business Problem
The Coffee Bean Shop lacks a unified and interactive view of sales performance, cutomer geography, product prefernce, loyalty impact and seasonal/monthly trends across 2019-2022. Making it difficult for the business owner to quickly identify revenue drivers optimize inventory and product mix, targrt high -value markets, understand loyalty effects, and spot seasonal opportunities and declines to drive informed descisions on pricing, promotions, stocking, and expansion. A centralized dashboard is needed to transform the rae data into actionable insights that support better strategic and operational descisions. 
   ---
## 3. Data Source
   Coffee Bean Sales Raw Dataset (multi-table) was obtained from an online data professional. It has three Excel sheets.
   #### Worksheet One: Orders Details
   - Order ID
   - Order Date
   - Customer ID,
   - Product ID
   - Quanitity 
   #### Worksheet 2: Customer Details
   - CustomerID
   - Customer Name
   - Email
   - Phone Number
   - Address Line 1
   - City
   - Country
   - Post Code
   - Loyalty Card 
   #### Worksheet 3: Product Details
   - Product ID
   - Coffee Type
   - Roast Type
   - Size
   - Unit Price
   - Price per 100g
   - Profit
     These Worksheets were imported into Power BI for transformation, modelling, and  report development.
   ##### Aggregated KPIs from the dashboard
   - Total Orders: 
   - Total Customers: 1000
   - Total Revenue: $45.13k
  
   ---
   
## 4. Data Cleaning and Transformation (Power Query)
### **Steps Completed**
1. Loaded the three worksheets into Power BI.
2. Checked for and handled blanks, nulls, and incorrect entries.
3. Standardized incorrect entries, including:   
    - Ara - Arabica
    - Rob - Robusta
    - Lib - Liberica
    - Exc - Excelsa
    - L - Light
    - M - Medium
    - D - Dark
4. Verified and corrected data types, ensuring dates, text, numbers, and currencies were properly assigned.
5. Checked for spelling errors and column name inconsistencies and corrected them.
6. Removed irrelevant columns.
7. Establish relationships between the Product Table and Order Table with the **Product ID** |
   Establish a relationship between the Customer Table and Order Table with the **Customer ID**

   These steps ensured a clean, accurate, and analysis-ready dataset.
   ---
## 5. Data Modelling
   A Star schema model was developed

### - Fact Table
### - Dimension Tables

This structure made the model efficient, scalable, and sufficient for DAX calculation.
---
## 6. DAX Measures Created
To support analysis, several measures are created: 



## 7. Dashboard Design & Visuals
### Overview Dashboard
This page provides a full snapshot and includes:
- 


Filter for:
- Loyalty Card
- Year
This page helps managers evaluate sales performance.

## Live Dashboard
[Click here to view the Power BI Report] ( 


   
   


## 9. Tools Used
  -  **Power BI Desktop** - data visualization and dashboard
       - [download here] (https://microsoft.com)
  -  **Power Query** - data cleaning
  -  **Data Modelling in Power BI** - Manage Relationships to ensure correct cordinality and cross-filter direction
  -  **DAX** - measures
  -  **PowerPoint** - Dashboard Template designing-
