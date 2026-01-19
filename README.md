# Coffee Bean Orders Analysis (Product, Loyalty, and Seasonal Trends Analysis)

## Table of Content
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
   Coffee Bean Sales Raw Dataset (multi-table) was obtained from an online data professional. It has three tables: Orders, Customers, and Products.
   Typical Columns: Order Date, Customer ID, Country, Loyalty card( Yes/ No), Coffee Type ( Arabica, Robusta, Liberica, Excelsa), Roast Type, Unit Price, Quantity, Revenue(Calculated)
   ##### Aggregated KPIs from the dashboard
   - Total Orders: 
   - Total Customers: 1000
   - Total Revenue: $45.13k
   ---
## Tools Used
  -  Power BI Desktop (Primary) - data visualization [download here] (https://microsoft.com)
  -  Power Query - data cleaning
  -  Data Modelling in Power BI - Manage Relationships to ensure correct cordinality and cross-filter direction
  -  DAX - measures
  -  PowerPoint - Dashboard Template designing

## Data Cleaning and Preparation
### **Steps Taken**
1. **Replaced values**
   Table.ReplaceValue(#"Replaced Value5","Exc","Excelsa",Replacer.ReplaceText,{"Coffee Type"})
   Table.ReplaceValue(#"Removed Columns","L","Light",Replacer.ReplaceText,{"Roast Type"})

2. **Removing Irrelevant Columns**
   
