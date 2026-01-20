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
An interactive dashboard analyzing coffee bean shop sales across countries, customer segments, product types, roast profiles, and seasonal trends. Built to uncover revenue drivers, customer behaviour, and optimization opportunities.
**Key Metrics at a glance**
- Total Revenue
- Total Orders
- Unique Customers

  ## Key Business Insights
  ### 1. 


Filter for:
- Loyalty Card
- Year
This page helps managers evaluate sales performance.

## Live Dashboard
[Click here to view the Power BI Report] ( <iframe title="Cofee Dataset" width="600" height="373.5" src="https://app.powerbi.com/view?r=eyJrIjoiNTRhNDVjMDQtYTQ1YS00Yjg5LTk1ODItNzVmYjM2YWVmNDBlIiwidCI6IjhlYTkzODI3LWM1NTktNDBkZC1iNGFkLTcwYWQ4YjBiYjhiZSJ9" frameborder="0" allowFullScreen="true"></iframe> )


   
   
---
## 8. Key Insights from the Dashboard

### Overall Performance Snapshot
- Total Revenue: ≈ $20.92K 
- Total Orders: 479
- Total Unique Customers: 479  
  → Every customer made exactly one order on average (low repeat purchase behavior → strong opportunity to improve customer retention)

### Customer & Market Geography
- Dominant market: United States generates the vast majority of revenue/customers (0.37M in the bar chart scale — most likely $370K if mis-scaled labels or $18–19K realistic given total)
- Ireland — second place ($6–8K range)
- United Kingdom — distant third ($2–3K range)
  
→ Business is heavily US-dependent (80–90% of revenue). Very limited geographic diversification → high risk if the US market softens.

### Loyalty Program Effectiveness
- Loyalty Card holders (Yes): significantly fewer customers than non-holders.
- Non-loyalty customers drive much higher total revenue .

→ Loyalty program underperforming  
→ Urgent opportunity: increase sign-ups + analyze whether loyalty members have higher LTV (lifetime value) over multiple purchases.

### Product Performance — Coffee Types
- Revenue ranking (highest to lowest):
1. Excelsa — $6.1K
2. Arabica — $5.4K
3. Liberica — $5.2K
4. Robusta — $4.2K

- Customer count (who bought each type at least once):
1. Excelsa — 132
2. Arabica — 122
3. Robusta — 118
4. Liberica — 107

→ Excelsa leads both in revenue and number of customers — currently the star product.  
→ Robusta lags noticeably — lowest revenue and fewest buyers → candidate for review (phase out? reposition? bundle?).

### Roast Type Preference
Revenue contribution (donut chart — percentages very close):
- Light roast — ~35.4% ($7.41K)
- Medium roast — ~33.6% ($7.03K)
- Dark roast — ~30.96% ($6.48K)

→ Very balanced preference, i.e no extreme skew.  
→ Light roast has a slight edge, trend worth watching if health/clean-taste narratives continue to grow.

### Seasonal / Time Trends
- Revenue shows clear seasonality with multiple peaks and troughs across months
- Highest points appear around the March–May and October–November periods
- Noticeable dips in July–August and around December–January

→ Classic coffee seasonality pattern (stronger in cooler/spring months in Northern Hemisphere markets).  
→ Opportunity: run promotions during low periods (summer/back-to-school dip).








---

## 9. Tools Used
  -  **Microsoft Power BI** - data visualization and dashboard
       - [download here] (https://microsoft.com)
  -  **Power Query Editor** - data cleaning
  -  **Star Schema Data Model** - Manage Relationships to ensure correct cordinality and cross-filter direction
  -  **DAX(Data Analysis Expression)** - measures
  -  **PowerPoint** - Dashboard Template designing

---
##10. Project Deliverables







---
#11. Potential extensions

Drawing from the coffee Bean sales data (2019–2022), here are targeted extension opportunities. These focus on leveraging strengths (e.g., Excelsa dominance, the US market) while addressing weaknesses (e.g., low repeats, geographic concentration). I've prioritized them by feasibility and potential ROI, assuming a small-to-medium coffee business sales (e.g., roastery or online shop) with ~$21K annual revenue and one-time buyers.

#### 1. Geographic Market Expansion (High Priority)
   - Why? The US accounts for ~85–90% of revenue, with Ireland and the UK as minor contributors. This heavy reliance poses risk from US-specific factors (e.g., economic shifts or competition).
   - Extensions Ideas:
     - Enter adjacent markets: Target Canada or EU countries (e.g., Germany, France) with similar coffee cultures. Start with low-cost e-commerce shipping or partnerships.
     - Localized marketing: Use digital ads geo-targeted to Ireland/UK to boost their share from 10–15% to 30%. Test pop-up shops or wholesale to local cafes.
     - Expected Impact: Could double revenue in 1–2 years by diversifying to 50% non-US, assuming similar AOV ($44/order).
   - Data Tie-In: Bar chart shows untapped potential in non-US regions—scale up from current low volumes.

#### 2. Product Line Extensions (Medium-High Priority)
   - Why? Excelsa leads in revenue ($6.1K) and customers (132), while roasts are balanced (Light slightly ahead at 35%). Robusta lags ($4.2K), indicating room for innovation without overhauling the core lineup.
   - Extension Ideas:
     - New blends/varieties: Introduce Excelsa-based hybrids (e.g., Excelsa-Arabica blend) or flavored options (e.g., vanilla Light roast) to capitalize on top performers.
     - Related products: Expand beyond beans/grounds to accessories (e.g., brew kits, mugs) or ready-to-drink (e.g., cold brew concentrates). Bundle with underperformers like Robusta to lift its sales.
     - Sustainable/niche lines: Add organic or fair-trade certifications, especially for Light roasts, aligning with trends toward healthier options.
     - Expected Impact: 20–30% revenue uplift by cross-selling to existing customers, turning one-time buyers into repeats.
   - Data Tie-In: Revenue by coffee/roast types highlights winners (Excelsa/Light) for safe experimentation; customer counts show broad appeal but room for deeper engagement.

#### 3. Loyalty & Retention Program Overhaul (High Priority)
   - Why? Non-loyalty customers drive most revenue, and with 479 customers matching 479 orders, repeat business is minimal (average 1 order/person).
   - Extension Ideas:
     - Subscription model: Offer monthly coffee boxes (e.g., "Excelsa Explorer" with rotating roasts) at a discount for loyalty members.
     - Tiered rewards: Extend program with points for referrals, reviews, or social shares—integrate app-based tracking for personalization.
     - Partnerships: Collaborate with complementary brands (e.g., tea or snack companies) for co-branded loyalty perks.
     - Expected Impact: Boost repeat rate to 20–30%, potentially adding $5–10K annual revenue from existing base.
   - Data Tie-In: Loyalty bar chart reveals underutilization—fixing this directly addresses the one-and-done customer pattern.

#### 4. Seasonal & Promotional Strategies (Medium Priority)
   - Why? Revenue peaks in spring (March–May) and fall (Oct–Nov), with dips in summer (July–Aug) and winter holidays (Dec–Jan), suggesting weather-driven or holiday-related demand.
   - Extension Ideas:
     - Seasonal limited editions: Launch summer iced blends (e.g., Light roast cold brew) or holiday gift sets to flatten dips.
     - Event-based extensions: Tie into coffee events (e.g., virtual tastings) or pop-ups during peaks; use email/SMS campaigns for off-season discounts.
     - Data-driven forecasting: Integrate inventory tools to overstock peaks and promo-clear lows.
     - Expected Impact: Stabilize monthly revenue by 10–15%, reducing volatility.
   - Data Tie-In: Line chart clearly maps trends—extensions here are low-risk, quick wins.

#### 5. Digital & Operational Enhancements (Medium Priority)
   - Why? Low repeats and balanced products suggest untapped online potential; data doesn't show channels, but implies e-commerce focus given geographic spread.
   - Extension Ideas:
     - E-commerce upgrades: Add personalization (e.g., roast quizzes) or AI recommendations based on past buys.
     - Analytics integration: Extend to track post-2022 data (e.g., via Google Analytics) for real-time insights.
     - Sustainability focus: If data hints at premium buyers (e.g., Excelsa appeal), extend to eco-packaging or carbon-neutral shipping.
     - Expected Impact: Improve conversion rates by 15–20%, supporting all other extensions.
   - Data Tie-In: Overall metrics (e.g., unique customers = orders) scream for better retention tech.













