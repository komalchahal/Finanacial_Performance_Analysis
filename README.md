Finanacial_Performance_Analysis
# Financial Performance Analysis Dashboard (Power BI Case Study)

## Project Overview
This project is a comprehensive Financial Performance Dashboard created for "The Finance Group." The goal was to provide an executive-level summary of the company's financial health, focusing on profitability, budget compliance, cash flow, and operational efficiency.

The dashboard allows stakeholders to monitor key performance indicators (KPIs) and perform root-cause analysis using interactive visuals and drill-down features.

## 📊 Live Dashboard Preview
> *Tip: After uploading your screenshot to GitHub, replace the placeholder below with your image link.*
![Dashboard Screenshot](path/to/your/screenshot.png)

## 🎯 Key Requirements & Features
As per the project requirements, the following features were implemented:
- KPI Cards: Real-time tracking of Total Revenue, Gross Margin %, EBITDA %, and Net Cash.
- Financial Trends: Monthly Revenue vs. Profitability (Gross Profit & EBITDA) analysis.
- Budget vs. Actual: Regional variance analysis with conditional formatting.
- Cash Flow Analysis: A Waterfall chart visualizing monthly net cash movement.
- Operational Efficiency: Average Receivables and Payables aging trends.
- Interactive Filtering: Slicers for Region, Product Category, and Date Range.
- AI-Driven Insights: Decomposition Tree for root-cause analysis of profit drivers.

## 🛠️ Tools & Technologies Used
- Power BI Desktop: For data modeling and visualization.
- DAX (Data Analysis Expressions): Created advanced measures for margins, variance %, and average aging days.
- Power Query: Performed data cleaning, data type transformations, and calendar table creation.

## 📉 Key Business Insights
- Revenue Shortfall: The company missed revenue targets across all regions, with the South Region showing the highest variance of -27%.
- Profitability Strength: Despite missing volume targets, the company maintained a strong Gross Margin of 45.55% and EBITDA of 25%.
- Balanced Cash Cycle: Average Receivables and Payables are aligned at ~30 days, indicating a healthy and sustainable cash conversion cycle.
- Liquidity: The company ended the period with a positive Net Cash position of $688K.

## 🧠 DAX Formulas Used
`dax
Gross Margin % = DIVIDE(SUM(Data[Gross Profit]), SUM(Data[Revenue]))

Revenue Variance % = DIVIDE([Total Revenue] - SUM(Data[Revenue Budget]), SUM(Data[Revenue Budget]))

Net Cash Flow = SUM(Data[Cash Inflows]) - SUM(Data[Cash Outflows])
