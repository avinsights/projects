Global Energy Consumption & Savings Analysis (Tableau)

Problem Statement : This dashboard was developed to provide an interactive visualization of global energy consumption patterns and the financial effectiveness of renewable energy adoption. Organizations and environmental agencies often struggle to analyze high-volume energy data stored in cloud warehouses like Snowflake.

This Tableau-powered solution bridges that gap by connecting directly to cloud data sources to monitor energy usage (kWh) and cost savings (USD) across different regions, countries, and energy sources. By identifying which energy types (Solar, Wind, Hydro, etc.) yield the highest savings and which regions are leading in adoption, stakeholders can make informed decisions to optimize sustainability initiatives and financial subsidies.

Steps Followed

Step 1: Established a live connection between Tableau Desktop and a Snowflake data warehouse (yoqzkjs-lc53065.snowflakecomputing.com).

Step 2: Navigated to the TABLEAU_DATA schema to extract the ENERGY_CONSUMPTION dataset for analysis.

Step 3: Conducted data profiling within Tableau to ensure correct data roles for dimensions like Region, Country, and Energy Source, and measures like Monthly Usage (kWh) and Cost Savings (USD).

Step 4: Developed time-series visualizations to track energy adoption trends based on the Adoption Year and Year columns.

Step 5: Built comparative bar charts and maps to analyze KWH Usage and Cost Savings across geographic hierarchies (Region > Country).

Step 6: Integrated filters for Income Level, Urban/Rural classification, and Subsidy Status to allow for granular user-driven exploration.

Step 7: Designed specific worksheets to compare the performance of different Energy Sources, identifying which technologies provide the best ROI for households.

Step 8: Created a cohesive dashboard layout that combines geographic insights with financial performance metrics for a 360-degree operational view.

Step 9: Optimized the workbook performance by managing Snowflake's COMPUTE_WH warehouse settings for real-time query execution.

Key Measures & Metrics

Total Energy Volume: Represented by the sum of MONTHLY_USAGE_KWH across all households.

Financial Impact: Calculated through the COST_SAVINGS_USD metric to measure the economic benefit of renewable transitions.

Adoption Scale: Tracked using the count of HOUSEHOLD_ID and segmented by HOUSEHOLD_SIZE.

Policy Efficiency: Measured by comparing savings and usage for households marked with SUBSIDY_RECEIVED.

Insights Based on the visual analysis of the Snowflake-integrated data, the following strategic inferences were drawn:

[1] Geographic Savings & Usage

Regional Performance: Analysis of the "Cost Savings USD By Region" worksheet reveals which continents are realizing the highest financial benefits from green energy.

National Benchmarking: The "KWH By Country" visualization identifies top-consuming nations, providing a roadmap for where energy efficiency programs are most needed.

[2] Energy Source ROI

Resource Efficiency: By comparing "KWH By Energy Source" and "Cost Savings Usd By Energy Source", the dashboard highlights which energy types (e.g., Wind vs. Solar) offer the best balance of high output and high savings.

Technological Adoption: Insights from these visuals help determine if localized energy sources (like Biomass or Geothermal) are outperforming more common sources in specific regions.

[3] Socio-Economic Trends

Income & Location Dynamics: Using filters for Income Level and Urban/Rural, the dashboard shows how energy adoption differs between low-income rural areas and high-income urban centers.

Subsidy Impact: The data allows for a direct comparison of whether government subsidies significantly increase cost savings or if organic market factors are the primary drivers.
