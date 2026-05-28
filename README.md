# Financial Performance Analysis Case Study

## Project Overview

This project is a comprehensive Financial Performance Dashboard created for "The Finance Group." The goal was to provide an executive-level summary of the company's financial health, focusing on profitability, budget compliance, cash flow, and operational efficiency.

The dashboard allows stakeholders to monitor key performance indicators (KPIs) and perform root-cause analysis using interactive visuals and drill-down features.

Live Dashboard Preview

<img width="1465" height="731" alt="Screenshot (64)" src="https://github.com/user-attachments/assets/6dcf87a5-2603-4d0b-bd78-a2c92d309a58" />

## Key Requirements & Features

As per the project requirements, the following features were implemented:

- KPI Cards: Real-time tracking of Total Revenue, Gross Margin %, EBITDA %, and Net Cash.
- Financial Trends: Monthly Revenue vs. Profitability (Gross Profit & EBITDA) analysis.
- Budget vs. Actual: Regional variance analysis with conditional formatting.
- Cash Flow Analysis: A Waterfall chart visualizing monthly net cash movement.
- Operational Efficiency: Average Receivables and Payables aging trends.
- Interactive Filtering: Slicers for Region, Product Category, and Date Range.
- AI-Driven Insights: Decomposition Tree for root-cause analysis of profit drivers.

## Tools & Technologies Used

- Power BI Desktop: For data modeling and visualization.
- DAX (Data Analysis Expressions): Created advanced measures for margins, variance %, and net cash flow.
- Power Query: Performed data cleaning, data type transformations, and calendar table creation.

## Key Business Insights

- Revenue Shortfall: The company missed revenue targets across all regions, with the South Region showing the highest variance of -27%.
- Profitability Strength: Despite missing volume targets, the company maintained a strong Gross Margin of 45.55% and EBITDA of 25%.
- Balanced Cash Cycle: Average Receivables and Payables are aligned at ~30 days, indicating a healthy and sustainable cash conversion cycle.
- Liquidity: The company ended the period with a positive Net Cash position of $688K.

 ## DAX Formulas Used
 
•	Gross Margin %: Divide(sum(Data[Gross Profit]),sum(Data[Revenue]),0) - Measures core production efficiency. 

•	Revenue Variance %: DIVIDE(sum(data[Revenue])-sum(Data[Revenue Budget]),sum(Data[Revenue Budget]),0) - Highlights the percentage deviation from set financial   targets. 

•	EBITDA% = Divide(sum(Data[EBITDA]),sum(Data[Revenue]))

•	Net Cash Flow: Sum(Data[Cash Inflows])-sum(Data[Cash Outflows]) - Tracks actual liquidity available at the end of each period
