Global Retail Sales Performance Report

Dashboard Link: https://app.powerbi.com/links/sECxiX8I5T?ctid=ebef2c48-9d23-48db-8a26-ad3693e2df80&pbi_source=linkShare

Problem Statement : This dashboard was developed to provide an end-to-end analysis of global retail sales, inventory health, and regional market trends. In a highly competitive retail environment, businesses often struggle with fragmented data that makes it difficult to track real-time performance across diverse product categories and geographic locations.

This tool centralizes sales data to help leadership monitor key performance indicators (KPIs) such as total revenue, profit margins, and year-over-year growth. By identifying top-selling products and underperforming regions, the business can optimize its supply chain, adjust pricing strategies, and target specific customer demographics more effectively to drive sustainable growth.

Steps Followed

Step 1: Ingested high-volume retail sales datasets into Power BI Desktop from a combination of SQL databases and CSV flat files.

Step 2: Utilized Power Query Editor to conduct thorough data profiling, checking for column distribution and quality to ensure data accuracy across thousands of records.

Step 3: Performed extensive data cleaning, including standardizing date formats, handling null values in discount columns, and creating custom categories for product lines.

Step 4: Developed a robust Star Schema data model to ensure efficient query performance and accurate relationships between Sales, Products, and Geography tables.

Step 5: Implemented a professional visual theme to maintain brand consistency and ensure the dashboard is accessible for executive decision-making.

Step 6: Integrated Advanced Slicers for "Region," "Category," "Segment," and "Order Date" to allow stakeholders to perform multi-dimensional drill-downs.

Step 7: Developed complex DAX measures to calculate essential retail metrics, including Total Sales, Profit Margin %, Total Quantity Sold, and Average Order Value.

Step 8: Created geographic map visuals to represent sales density and identify emerging market opportunities across global territories.

Step 9: Published the final report to the Power BI Service, enabling automated data refreshes and secure sharing across the organization.

Key DAX Measures & Columns Revenue Performance:

Total Sales = SUM(Sales_Data[Sales_Amount])

Profitability Tracking:

Total Profit = SUM(Sales_Data[Profit])

Order Volume:

Total Quantity = SUM(Sales_Data[Quantity])

Efficiency Metric:

Profit Margin % = DIVIDE([Total Profit], [Total Sales]) * 100

Insights A deep dive into the sales data yields several critical business inferences for strategic planning:

[1] Sales & Profitability Overview

Revenue Leaders: Identified the top-performing product categories that contribute to the majority of total revenue.

Margin Analysis: Pinpointed specific products with high sales volume but low profit margins, signaling a need for pricing or supplier renegotiation.

[2] Regional Market Trends

High-Growth Regions: Data reveals specific geographic zones experiencing significant year-over-year sales growth.

Inventory Optimization: Correlated regional sales trends with inventory levels to reduce stockouts in high-demand areas.

[3] Customer Segment Behavior

Primary Segments: Analyzed purchasing patterns across B2B and B2C segments to tailor marketing campaigns.

Seasonality: Uncovered peak sales periods throughout the year, allowing for better workforce and resource planning during high-traffic months.
