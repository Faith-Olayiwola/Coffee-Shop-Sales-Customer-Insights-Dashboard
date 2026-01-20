# Coffee Bean Orders Analysis (Product, Loyalty, and Seasonal Trends Analysis)

## Table of Contents
1. Project Overview 
2. Data Source
3. Tools
4. Data Cleaning and Preparation
5. Objectives of the Project
6. Results and Findings
7. Recommendations and Conclusion

   ---
   ## Project Overview
   This Project demonstrates end-to-end data collection and analysis skills, followed by data cleaning in **Power Query**, and finally performing explorative analysis and visualization in **Power Bi.**
   Interactive Power BI dashboard analyzing coffee bean sales to identify top-performing products, geographic revenue drivers, loyalty program effectiveness, and seasonal revenue fluctuations. Supports inventory decisions, marketing targeting, and retention strategies for a coffee retailer. 

   ---
   ## Data Source
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
## Tools Used
  -  **Power BI Desktop** - data visualization and dashboard
       - [download here] (https://microsoft.com)
  -  **Power Query** - data cleaning
  -  **Data Modelling in Power BI** - Manage Relationships to ensure correct cordinality and cross-filter direction
  -  **DAX** - measures
  -  **PowerPoint** - Dashboard Template designing

## Data Cleaning and Transformation
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
6. Establish relationships between the three dataset wroksheet in the Power Bi Model:
   - 
8.  
1. **Data Loading and Inspection**
2. **Handling Missing Values** and replaced nulls 
3.  **Replaced values**
   Table.ReplaceValue(#"Replaced Value5","Exc","Excelsa",Replacer.ReplaceText,{"Coffee Type"})
   Table.ReplaceValue(#"Removed Columns","L","Light",Replacer.ReplaceText,{"Roast Type"})

4. **Removing Irrelevant Columns**
5. **Explorative Data Analysis**
   
