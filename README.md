# Eliminating-Data-Silos-with-Advanced-SQL-ETL
A comprehensive ETL and data architecture project designed to aggregate disparate business data into a centralized "Source of Truth" for real-time KPI tracking and strategic decision-making.
---
## Table of Contents
- Project Overview
- Data Sources
- Tools & Technology
- Data Cleaning & ETL Process
- Exploratory Data Analysis (EDA)
- Advanced SQL Analysis
- Results & Business Impacts
- Recommendations
- Limitations

## Project Overview
This project focuses on solving the "Data Silo" problem for Vacat, an e-commerce company. The objective was to aggregate data from three disparate sources—PostgreSQL, Salesforce, and ERP systems—into a centralized platform. By performing complex ETL processes and building a unified relational data model, I automated manual reporting workflows, enabling executive leadership to derive real-time insights into sales performance, customer behavior, and operational efficiency.

## Data Sources
- PostgreSQL: Product catalog, inventory  
- Salesforce: Customer & segmentation  
- ERP: Transactions & fulfillment  

---

## Tools & Technology
- SQL (PostgreSQL): For complex data extraction, transformation, and load (ETL) logic.
- GenAI (LLM/RAG): Leveraged to accelerate schema mapping and automate initial data cleaning.
- Power BI: For data modeling (DAX) and developing a 5-view interactive dashboard solution.
- Microsoft Excel: For initial data auditing and validation.

## Data Cleaning and Preparation
The data preparation phase involved a multi-stage pipeline:
- Data Loading & Schema Mapping: Used GenAI to align column headers and data types across the three disparate systems.
- Handling Missing Values & Duplicates: Conducted rigorous SQL audits to remove duplicate customer IDs and handle null revenue values.
- Standardization: Normalized regional names and product categories to ensure a consistent join between CRM and ERP tables.

## Exploratory Data Analysis (EDA)
I performed an automated EDA to identify trends, rankings, and outliers:
- Univariate Analysis: Analyzed sales distribution to identify the KPIs.
- Bivariate Analysis: Correlated "Late Shipments" with "Order Volume" to find profit-draining operational bottlenecks.
- Multivariate Analysis: Segmented customer purchasing patterns by demographic and behavioral factors.

## Data Analysis
I utilized Advanced **SQL** to transform the raw data into actionable insights and **Power BI** to visualize the insights:
- Common Table Expressions (CTEs): Modularized the cleaning and joining logic to ensure the script is scalable and maintainable.
- DAX Modeling: Engineered primary and secondary metrics in Power BI to automate YoY growth and Margin calculations.

## Results & Business Impacts
- Revenue Growth: Generated $1.8M revenue with 68% growth and 13% profit margin
- Regional Insight: West led in revenue, but East was most profitable
- Customer Segment: Millennials delivered highest profitability (48%) despite lower sales than Gen X
- Product & Ops Impact: Top products drove volume, but late shipments reduced revenue/profit
- Forecast: Revenue projected to reach ~$3M in next 10 months
  
<img width="1676" height="921" alt="image" src="https://github.com/user-attachments/assets/aa5104b7-743e-4044-8e4b-97d3196a9c99" />

<img width="1579" height="924" alt="image" src="https://github.com/user-attachments/assets/290135fb-f488-4943-90ee-158bf6686d6d" />


## Recommendations
- Increase marketing campaigns in the East region.
- Create targeted promotions for Millennials (25–35).
- Personalize offers and loyalty programs for this segment.
- Optimize logistics operations in other to improve on the late shipment as this impacts sales and profit.

## Limitations
- Data Integration Constraints: Source systems (PostgreSQL, CRM, ERP) had inconsistent schemas and potential data quality issues, which impacted initial analysis and required data cleansing.
- Model Assumptions: Revenue forecast assumes historical trends remain constant, limiting reliability under changing market conditions or customer behavior.
