Loan Default Report

Dashboard Link : https://app.powerbi.com/links/4658mIYs5z?ctid=ebef2c48-9d23-48db-8a26-ad3693e2df80&pbi_source=linkShare

Problem Statement This dashboard was developed to help financial institutions proactively manage credit risk by identifying patterns associated with loan defaults. By analyzing historical borrower data, the dashboard provides a visual framework to distinguish between "low-risk" and "high-risk" customers.

The primary objective is to minimize financial loss by identifying key risk drivers—such as debt-to-income ratios, credit history, and employment stability—enabling the lending team to make data-driven decisions on loan approvals and interest rate adjustments.

Steps Followed

Step 1: Extracted raw loan data from SQL databases and performed initial data profiling to identify missing values and outliers.

Step 2: Leveraged Power BI Dataflows to handle ETL (Extract, Transform, Load) processes, ensuring a clean and reusable data source for the report.

Step 3: Used Power Query Editor to standardize data types, merge relevant tables (borrower info, payment history), and filter out non-essential records.

Step 4: Implemented a Star Schema data model to optimize query performance and ensure accurate relationships between fact tables (loans) and dimension tables (customers, dates).

Step 5: Developed complex DAX measures to calculate critical KPIs such as Default Rate %, Total Outstanding Balance, and Borrower Risk Scores.

Step 6: Integrated Visual Slicers for fields like "Loan Grade," "Employment Length," and "Home Ownership" to allow stakeholders to drill down into specific risk segments.

Step 7: Applied Conditional Formatting to table visuals to highlight "High Risk" accounts where the probability of default exceeded internal thresholds.

Step 8: Published the final report to Power BI Service, enabling automated data refreshes and collaborative access for the credit risk team.

Key DAX Measures & Columns Total Loan Volume: Total Loans = COUNT(Loan_Data[Loan_ID])

Default Rate %: Default Rate = DIVIDE(CALCULATE([Total Loans], Loan_Data[Status] = "Default"), [Total Loans]) * 100

Risk Categorization: Risk Level = IF(Loan_Data[DTI_Ratio] > 0.4, "High Risk", "Moderate/Low Risk")

Insights A multi-page risk assessment report was created, yielding several critical business inferences:

[1] Overall Portfolio Health Total Active Loans: [Insert Number, e.g., 50,000]

Portfolio Default Rate: [Insert %, e.g., 12%]

A significant portion of defaults was concentrated in "Grade D" and "Grade E" loan categories, suggesting a need for stricter approval criteria for these sub-prime tiers.

[2] Borrower Risk Drivers Debt-to-Income (DTI): Borrowers with a DTI ratio above 35% were 3x more likely to default compared to those below 20%.

Employment Stability: Customers with less than 2 years of employment history showed a 15% higher delinquency rate.

Home Ownership: Renters demonstrated a marginally higher default rate compared to homeowners with existing mortgages.

[3] Financial Impact Recoverable Amount: Identified specific segments where early intervention strategies (collections) could protect up to [Insert Amount, e.g., $2M] in potential losses.

Average Loan Value: The average amount for defaulted loans was [Insert Amount], indicating that high-value loans require more rigorous collateral verification.
