UPI Transaction Analysis Report

Dashboard Link: https://app.powerbi.com/links/2kqcoyPgmr?ctid=ebef2c48-9d23-48db-8a26-ad3693e2df80&pbi_source=linkShare

Problem Statement : This dashboard was developed to provide a comprehensive analysis of Unified Payments Interface (UPI) transactions, focusing on digital payment adoption, transaction success rates, and user spending behavior. In the rapidly evolving fintech landscape, understanding the flow of digital micro-payments and larger commercial transfers is essential for financial institutions and payment service providers.

This tool centralizes high-volume UPI data to help stakeholders monitor real-time transaction volumes, track the average value of "Person-to-Person" (P2P) versus "Person-to-Merchant" (P2M) payments, and identify regional hotspots for digital adoption. By analyzing transaction failure points and peak usage times, the business can optimize server infrastructure, enhance user experience, and drive strategic growth in the digital payments ecosystem.

Steps Followed

Step 1: Ingested large-scale UPI transactional datasets into Power BI Desktop from secure cloud databases and flat files.

Step 2: Utilized Power Query Editor to conduct thorough data profiling, checking for column distribution and quality to ensure data integrity across millions of transaction records.

Step 3: Performed extensive data cleaning, including standardizing bank-specific transaction codes and handling null values in the "Status" column to ensure accurate success/failure reporting.

Step 4: Developed a robust Star Schema data model to ensure efficient query performance between the main Transaction fact table and dimension tables like Banks, Users, and Dates.

Step 5: Implemented a professional fintech-inspired visual theme to maintain clarity for operational teams and executive leadership.

Step 6: Integrated Advanced Slicers for fields such as "Bank Name," "Transaction Status," "Region," and "Payment Type" to allow for multi-dimensional deep-dives.

Step 7: Developed complex DAX measures to calculate critical fintech KPIs, including Total Transaction Value, Success Rate %, Average Transaction Value, and User Growth.

Step 8: Created geographic map visuals to represent digital payment density and identify regions with high growth potential for UPI services.

Step 9: Published the final report to the Power BI Service, enabling real-time monitoring of transaction health and secure sharing across the organization.

Key DAX Measures & Columns Volume Performance:

Total Transaction Value = SUM(UPI_Data[Transaction_Amount])

Network Reliability:

Success Rate % = DIVIDE(CALCULATE(COUNT(UPI_Data[ID]), UPI_Data[Status]="Success"), COUNT(UPI_Data[ID])) * 100

Activity Scale:

Total Transaction Count = COUNT(UPI_Data[Transaction_ID])

User Engagement:

Avg Value Per Transaction = DIVIDE([Total Transaction Value], [Total Transaction Count])

Insights A deep dive into the UPI transaction data yields several critical business inferences for strategic growth:

[1] Network & Success Performance

Reliability Benchmarks: Identified the overall network success rate, pinpointing specific banking partners or time periods where failure rates spiked.

Failure Analysis: Analyzed the primary reasons for transaction failures (e.g., technical error vs. insufficient funds) to target technical improvements.

[2] Spending & User Trends

High-Activity Zones: Data reveals specific regions and urban centers where UPI adoption and transaction density are highest.

Usage Patterns: Uncovered peak transaction periods throughout the day, allowing for better management of server loads during high-traffic hours.

[3] Payment Category Behavior

Merchant vs. Personal: Analyzed the split between P2P and P2M transactions to understand how UPI is being used for daily retail payments.

Transaction Tiering: Grouped transactions into value brackets to identify the volume of micro-payments versus large-ticket transfers.
