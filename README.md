# CUSTOMER-BEHAVIOR-REVENUE-INTELLIGENCE-BUSINESS-OPTIMIZATION-using-Python
### 1. PROJECT OVERVIEW
This capstone project investigates customer purchasing behavior, sales performance, product contribution, regional results, discount effectiveness, and customer retention for a fictional fast-growing Nigerian retail chain, Orion Retail Intelligence Group. 
The business scenario describes a retailer selling Electronics, Fashion, Home Appliances, and Groceries across major Nigerian cities. Leadership has observed slower revenue growth, inconsistent purchasing behavior, regional performance differences, possible discount-related pressure, and customers who do not return after their first purchase.
The purpose of the analysis is to transform customer, product, and order data into practical business intelligence that can support revenue growth, customer retention, product planning, and operational decisions.
### 2. Business Problem
Management needs a clear view of what drives revenue and repeat purchasing, which regions and products perform best, how customer segments differ, and whether discounting is associated with stronger sales outcomes. The analysis is designed to answer these questions using a structured end-to-end analytics workflow.
### 3. Project Objectives
* Consolidate customer, product, and order records into one analysis-ready dataset.
* Assess data quality by checking structure, missing values, duplicates, and data types.
* Measure core sales KPIs, including revenue, orders, customers, and quantity sold.
* Compare revenue, order volume, and average order value across regions.
* Identify high- and low-performing products and categories.
* Understand spending and purchase frequency across customer segments and age groups.
* Evaluate monthly revenue and order trends for possible seasonality.
* Examine relationships between discount levels, quantity sold, and revenue.
* Measure repeat-customer and one-time-buyer rates.
* Assess revenue concentration among the highest-value customers.
* Develop customer value segments using revenue and purchase frequency.
* Translate findings into actionable business recommendations.
### 4. Tools Used
1. Python — data processing, feature engineering, aggregation, and analysis.
2. Pandas — data import, cleaning, joining, grouping, and KPI calculation.
3. Matplotlib — business charts and visual storytelling.
4. Excel — source data supplied as a workbook containing three sheets.
### 5. Dataset Description
The source workbook is described as containing three relational tables:
* Customers: Customer_ID, Gender, Age, Region/city information, Customer_Segment, and Signup_Date.
* Products: Product_ID, Product_Name, Category, and Unit_Price.
* Orders: Order_ID, Customer_ID, Product_ID, Order_Date, Quantity, Discount, Revenue, and Payment_Method.
The tables are linked through Customer_ID and Product_ID. The final analytical dataset should combine customer attributes, product details, and order-level information.
### 6. Analytical Approach & Workflow
* Phase 1 — Data Import & Integration: Load the Customers, Products, and Orders sheets; inspect row counts, columns, data types, missing values, and duplicates; then join the tables using their relevant identifiers.
  
<img width="926" height="436" alt="image" src="https://github.com/user-attachments/assets/3bd9e86d-e0f6-4be0-803c-cc18eed59743" />

<img width="925" height="388" alt="image" src="https://github.com/user-attachments/assets/3b911a0e-2a94-40f9-8a7c-8d216d550e4a" />

<img width="933" height="431" alt="image" src="https://github.com/user-attachments/assets/b92fba10-1968-4491-9e97-1b803af53446" />

<img width="916" height="431" alt="image" src="https://github.com/user-attachments/assets/69115e62-5635-4d50-8057-f8a0ac365076" />

<img width="926" height="329" alt="image" src="https://github.com/user-attachments/assets/40526ef3-b3b4-4019-9794-abdd4d94b016" />

<img width="944" height="435" alt="image" src="https://github.com/user-attachments/assets/e7d1c723-db24-4eb8-8749-72142155f431" />

* Phase 2 — Data Cleaning & Feature Engineering: Convert Order_Date to a datetime field; derive year, month, and quarter; and calculate customer lifetime revenue, purchase frequency, revenue by region, and revenue-per-quantity. Average order value should be calculated as revenue per order, with the aggregation level clearly defined.

  <img width="935" height="396" alt="image" src="https://github.com/user-attachments/assets/7398efc4-2900-492c-b102-587d23563c23" />

  <img width="932" height="438" alt="image" src="https://github.com/user-attachments/assets/a1e927af-2da0-43e3-b161-ed939e6626c6" />

  <img width="911" height="365" alt="image" src="https://github.com/user-attachments/assets/42922f46-a845-4dae-a746-6bef7cfecf48" />

* Phase 3 — Exploratory Data Analysis: Calculate total revenue, total orders, unique customers, and total quantity sold. Review regional performance, category contribution, top and bottom products, customer segments, top 20 customers, age-group spending, and payment-method behavior.

<img width="912" height="383" alt="image" src="https://github.com/user-attachments/assets/1d38ce26-3536-41c7-abfd-d96933f4c035" />

<img width="913" height="289" alt="image" src="https://github.com/user-attachments/assets/47bae311-efce-407a-911a-3fa025d2b1c0" />

<img width="910" height="253" alt="image" src="https://github.com/user-attachments/assets/e5f9e84e-7329-4f6e-80c6-2880a1b9bcb5" />

<img width="921" height="388" alt="image" src="https://github.com/user-attachments/assets/9b4ee4ce-ccf7-41d6-aba7-9d577ec0282b" />

<img width="916" height="237" alt="image" src="https://github.com/user-attachments/assets/652a7c39-16e6-4883-b23b-7a5a5c657aab" />

* Phase 4 — Time-Series Analysis: Aggregate monthly revenue and order counts; identify the strongest and weakest months in the observed data; and investigate recurring patterns where the available time period supports a meaningful comparison.

<img width="913" height="439" alt="image" src="https://github.com/user-attachments/assets/203b8ce1-c89c-41f7-be2c-18afca1e6ee6" />

<img width="915" height="278" alt="image" src="https://github.com/user-attachments/assets/619970f1-65c5-4bc0-91b8-0bf57ff48657" />

* Phase 5 — Discount Effectiveness: Compare revenue and quantity sold across discount levels and assess the relationship between discount and revenue. Revenue alone does not establish profitability; margin or cost data would be needed to determine whether discounts improve profit.

<img width="910" height="296" alt="image" src="https://github.com/user-attachments/assets/e8649334-87d4-4451-8ddd-8e4a034f85bc" />

<img width="914" height="287" alt="image" src="https://github.com/user-attachments/assets/31b8e86f-b7a2-4241-8b10-e914fe073e1a" />

<img width="909" height="281" alt="image" src="https://github.com/user-attachments/assets/dc41906f-397e-4eba-8e31-952ae6438d8b" />

* Phase 6 — Customer Retention: Classify customers with more than one order as repeat customers. Calculate repeat-customer and one-time-buyer rates, and identify customers with consistently high purchase activity.

<img width="911" height="284" alt="image" src="https://github.com/user-attachments/assets/8fdc5899-cb0c-40ad-8c80-54ede2d516f6" />

<img width="919" height="409" alt="image" src="https://github.com/user-attachments/assets/578174dd-9192-4293-b9a1-984994c1cad4" />

<img width="915" height="403" alt="image" src="https://github.com/user-attachments/assets/76257ecb-2f3d-4f93-926f-32381e61ebdb" />

### Advanced — Customer Segmentation: Classify customers into High Value, Medium Value, and Low Value groups using total revenue and purchase frequency. Document the thresholds or rules used so the segmentation is reproducible.

<img width="913" height="433" alt="image" src="https://github.com/user-attachments/assets/ee9ba09e-b054-4001-a8bb-6d0ee9cc3aaf" />

<img width="919" height="433" alt="image" src="https://github.com/user-attachments/assets/b94a143f-c808-4443-906c-7ad59f603f35" />

### 8. Project Visualizations
1. Revenue by Region — bar chart.

  <img width="922" height="425" alt="image" src="https://github.com/user-attachments/assets/08614d95-ba6d-41a4-9339-cd07ed435979" />

2. Monthly Revenue Trend — line chart.
   
<img width="907" height="393" alt="image" src="https://github.com/user-attachments/assets/c82a021e-05b1-4032-abfa-d99972024724" />

<img width="923" height="431" alt="image" src="https://github.com/user-attachments/assets/e2bed06f-0a5d-4456-a802-efbc0411ad66" />

3. Revenue by Category — bar chart.

<img width="925" height="427" alt="image" src="https://github.com/user-attachments/assets/2993c6ee-5c52-42d4-ab55-7b0b4528390f" />

4. Top Products by Revenue — horizontal bar chart.

<img width="914" height="431" alt="image" src="https://github.com/user-attachments/assets/755cc19b-d1d9-41fa-b42c-51da4649efd9" />

5. Revenue by Customer Segment — pie chart.

<img width="913" height="432" alt="image" src="https://github.com/user-attachments/assets/c310cdee-58fb-48f1-8dff-a1af64bf1b6a" />

6. Spending by Age Group — bar chart.

<img width="919" height="425" alt="image" src="https://github.com/user-attachments/assets/c1d157f1-6d9d-4de3-96a9-0f9c72728e95" />

7. Discount vs Revenue — scatter plot.

<img width="924" height="439" alt="image" src="https://github.com/user-attachments/assets/ac3d6131-d2b8-48ed-9257-79cc0976372a" />

8. Monthly Order Trend — line chart.

<img width="910" height="322" alt="image" src="https://github.com/user-attachments/assets/f5562141-1df0-4a75-b51f-05dbb4246f68" />

<img width="920" height="434" alt="image" src="https://github.com/user-attachments/assets/5886c0cf-548f-4381-b4e8-ccbde0c5c1ba" />

### 9. KEY BUSINESS INSIGHTS
1. Revenue Performance: Analyzing revenue trends helps identify business growth patterns, sales fluctuations, and opportunities to improve financial performance.
2. Customer Behavior: Understanding customer purchasing habits reveals spending patterns, purchase frequency, and opportunities to improve customer engagement.
3. Product Performance: Evaluating product and category sales identifies high-performing products and those requiring further review or improvement.
4. Regional Performance: Comparing performance across geographical locations highlights differences in sales contribution and potential opportunities for market expansion.
5. Customer Segmentation: Analyzing customer groups reveals differences in spending patterns and purchasing frequency, supporting more targeted business strategies.
6. Customer Retention: Examining repeat purchases and one-time buyers helps assess customer loyalty and identify opportunities to strengthen long-term relationships.
7. Discount Effectiveness: Evaluating discount levels alongside revenue and sales volume helps assess promotional performance and potential effects on profitability.
8. Sales Trends and Revenue Concentration: Analyzing sales over time and revenue contributions across customers helps identify demand patterns and potential dependence on a small group of customers.

### 10. STRATEGIC BUSINESS RECOMMENDATIONS
* Improve Revenue Growth: Use sales performance data to identify growth opportunities, monitor revenue trends, and develop measurable sales improvement strategies.
* Strengthen Customer Relationships: Implement customer engagement initiatives, loyalty programmers’, and personalized offers to encourage repeat purchases and improve retention.
* Optimize Product Management: Allocate inventory based on demand patterns, product performance, stock availability, and profitability to improve operational efficiency.
* Develop Regional Growth Strategies: Evaluate regional performance, market demand, and operating costs to identify opportunities for expansion and improve underperforming locations.
* Implement Data-Driven Customer Segmentation: Group customers according to relevant characteristics, spending patterns, and purchase frequency to improve marketing effectiveness and resource allocation.
* Optimize Discount Strategies: Evaluate promotional campaigns using revenue, sales volume, and profit margins to ensure discounts contribute to sustainable business performance.
* Strengthen Sales Forecasting: Use historical sales data and observed trends to improve demand forecasting, inventory planning, budgeting, and resource allocation.
* Adopt Data-Driven Decision-Making: Develop interactive dashboards and regular performance reports to monitor key performance indicators, identify emerging issues, and support timely management decisions.


