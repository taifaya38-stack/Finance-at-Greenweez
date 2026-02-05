# Finance-at-Greenweez
🌱 Greenweez – Daily Profitability & Margin Analysis (Google Sheets)
🧠 Project Overview

Greenweez is an organic e-commerce platform operating in the B2C market, offering products that promote a healthier and more sustainable lifestyle.

This project was conducted in collaboration with the finance team, whose objective is to monitor daily profitability by analyzing the balance between revenue and multiple cost components.
The analysis was fully implemented in Google Sheets, following a structured, analyst-driven financial reporting approach.

🎯 Business Objective

The finance team requires a daily profitability report that enables them to:

- Monitor business performance on a daily basis

- Track the relationship between revenue and costs.

- Calculate and compare multiple types of margins.

- Identify cost drivers impacting profitability over time.

📊 Key Financial KPIs

Before analyzing the data, the following KPIs were defined:

- Margin = Revenue − Purchase Costs

- Margin Percentage

- Operational Margin (after logistics & shipping costs)

- Refund Margin

- Advertising Margin

- Final Margin (including refunds and advertising costs)

These metrics allow a progressive and realistic view of profitability.

📂 Data Sources

The analysis is based on four financial datasets:

- gwz_finance_orders – orders and revenue

- gwz_finance_campaign – advertising costs

- gwz_finance_shipping – logistics and shipping costs

- gwz_finance_refund – refunds and associated costs

Data was imported using manual CSV imports and IMPORTRANGE, depending on the source and update requirements.

🛠 Methodology

I. Data Import

- Manual import of campaign and refund CSV files.

- Automated imports using IMPORTRANGE() for orders and shipping.

- Initial exploration of columns and data completeness.

II. Data Cleaning

Several cleaning steps were required before analysis:

- Standardization of date formats across all datasets

- Creation of clean date columns using:

- SUBSTITUTE

- LEFT, LEN

- DATE, YEAR, MONTH, DAY

- Detection of anomalies and extreme values

- Investigation of abnormal purchase and logistics costs

- Handling limitations of IMPORTRANGE (filters & sorting)

III. Margin Calculations

1️⃣ Order Margin

- Gross margin = turnover − purchase cost

- Margin percentage calculated and formatted

2️⃣ Operational Margin

- Integration of logistics and shipping costs using XLOOKUP

Calculation of:

- Operational margin

- Operational margin percentage

3️⃣ Advanced Margins

- Refund margin (operational margin − refund costs)

- Advertising margin (operational margin − ads costs)

- Evaluation of how advertising impacts daily profitability

IV. Data Aggregation & Reporting

A daily profitability report was built using pivot tables:

1- Metrics aggregated by day include:

- Number of orders

- Total & average turnover

- Purchase costs

- Shipping & logistics costs

- Margins (gross, operational, ads-adjusted)

2- Advertising costs were added using XLOOKUP, and additional KPIs were computed:

- Ads margin

- Average ads margin per order

- Ads margin percentage

V. Refund Analysis (Advanced)

- Analysis of daily refund volume

- Calculation of refund delays

- Separation of refund aggregation from order dates

- Correct integration of refund costs based on refund date, not order date

- Final margin calculation including all cost components

📈 Key Outcomes

- Built a complete daily financial reporting system in Google Sheets

- Identified how logistics, refunds, and advertising impact margins

- Delivered actionable KPIs for the finance team

- Demonstrated strong data cleaning, aggregation, and financial modeling skills

🧪 Tools & Skills Used

- Google Sheets (advanced formulas & pivot tables)

- Data Cleaning & Transformation

- Financial KPI Modeling

- XLOOKUP / INDEX-MATCH

- Pivot Tables & Calculated Fields

- Business & Financial Analysis

🏁 Conclusion

This project demonstrates how structured data analysis and financial modeling can support profitability monitoring and decision-making in an e-commerce environment.
By progressively integrating costs and aggregating results at a daily level, the analysis provides a clear and realistic view of business performance.

👤 Author :Taif_Aya

Data Analyst – Academic / Portfolio Project
Focused on financial reporting and profitability analysis
