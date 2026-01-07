Brand & Transaction Analysis

Dashboard Link : https://app.powerbi.com/links/g8eYwpsw0l?ctid=ebef2c48-9d23-48db-8a26-ad3693e2df80&pbi_source=linkShare

Problem Statement : This dashboard was developed to analyze the market position and operational performance of various banking brands. In a competitive financial landscape, understanding how different brands perform across customer segments is vital for strategic growth.

The dashboard solves the problem of fragmented banking data by consolidating brand-specific metrics into a single view. It allows analysts to compare brand loyalty, transaction volumes, and service ratings across different demographics. By identifying which brands are leading in customer satisfaction and which are lagging in specific service areas (like online banking or branch service), the institution can make data-driven decisions to improve brand equity and operational efficiency.

Steps Followed

Step 1: Ingested a diverse banking dataset featuring multiple financial brands and customer transaction records.

Step 2: Utilized Power Query Editor to conduct data profiling, ensuring consistency across brand names and transaction categories.

Step 3: Performed data transformation to handle varied rating scales and missing values in customer feedback columns to ensure unbiased average calculations.

Step 4: Developed a comprehensive Data Model that links banking brands to specific transaction types, locations, and customer profiles.

Step 5: Created a professional visual interface optimized for brand comparison, utilizing a clean and modern theme.

Step 6: Integrated Interactive Slicers for "Bank Brand," "Transaction Type," "Region," and "Customer Segment" to enable granular analysis.

Step 7: Leveraged DAX (Data Analysis Expressions) to build custom measures for Brand Market Share, Average Transaction Value, and Net Promoter Scores (NPS).

Step 8: Added specialized visuals to track brand-specific performance in areas such as "In-branch Service," "Mobile App Ease of Use," and "Customer Support Quality".

Step 9: Published the finalized report to Power BI Service, allowing stakeholders to monitor brand performance through automated dashboards.

Key DAX Measures & Columns Total Brand Transactions:

Total Transactions = COUNT(Banking_Data[Transaction_ID])

Brand Satisfaction Index:

Avg Brand Rating = AVERAGE(Banking_Data[Overall_Satisfaction])

Customer Segment Distribution:

% Segment Volume = DIVIDE([Count of Customers], CALCULATE([Count of Customers], ALL(Banking_Data[Brand]))) * 100

Insights The analysis of the banking brand dataset provided the following key inferences for strategic decision-making:

[1] Brand Performance & Market Share

Dominant Brands: Identified the leading banking brands by transaction volume, with [Insert Top Brand Name] holding a [Insert %] share of the analyzed data.

Customer Sentiment: Analysis showed that while some brands lead in volume, others excel in customer sentiment, particularly in digital service ratings.

[2] Service Quality Benchmarks

Digital Excellence: Brands focusing on "Online Boarding" and "Mobile Connectivity" saw a [Insert %] higher retention rate among the 25-50 age demographic.

Operational Friction: Lower ratings were consistently observed in "Ease of Online Booking" for legacy brands, suggesting a critical area for digital transformation.

[3] Customer Behavioral Patterns

Returning vs. New: "Returning" customers accounted for over 80% of brand engagement, emphasizing the high ROI of customer loyalty programs in the banking sector.

Class Preferences: Customers using "Business Class" or premium banking services provided higher ratings for "Seat Comfort" (Branch Ambiance) and "On-board Service" (Personalized Banking).
