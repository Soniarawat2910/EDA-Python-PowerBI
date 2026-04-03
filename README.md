# **Project Name**    - USA Regional Sales Analysis

## 🗂️ **Project Summary**  
This EDA notebook dives into Acme Co.’s 2021–2025 USA sales dataset through:
Data Profiling & Cleaning: Verified schema, handled missing budgets, and corrected data types.
Univariate & Bivariate Analysis: Explored distributions (revenue, margin, unit price), product/channel/region breakdowns, and customer segments.
Trend & Seasonality: Charted monthly and yearly sales patterns, highlighting recurring surges and dips.
Outlier Detection: Identified extreme transactions at both ends of the revenue and unit-price spectra.
Correlation & Segmentation: Assessed relationships between key metrics and clustered customers by revenue vs. profit margin.

## ❓ **Problem Statement**  

Analyze Acme Co.’s 2021–2025 sales data to identify key revenue and profit drivers across products, channels, and regions; uncover seasonal trends and outliers; and align performance against budgets. Use these insights to optimize pricing, promotions, and market expansion for sustainable growth and reduced concentration risk.

## 🎯 **Objective**

Deliver actionable insights from Acme Co.’s 2021–2025 sales data to:
- Identify top-performing products, channels, and regions driving revenue and profit  
- Uncover seasonal trends and anomalies for optimized planning  
- Spot pricing and margin risks from outlier transactions  
- Inform pricing, promotion, and market-expansion strategies  
These findings will guide the design of a Power BI dashboard to support strategic decision-making and sustainable growth.

## 🎯 **Raw Data Structure**
Sales, products, budgets, customers, regions, and states were spread across unlinked tables. No relationships were defined initially— Pre-processing was required to clean, normalize, and join them for analysis.

![Raw Data Structure](Doc/Raw%20Data%20Structure.png)

## 🎯 **Final Dataset Structure – Ready for Analysis**

- Identifiers: order_number, order_date, customer_name, channel, product_name
- Financials: quantity, unit_price, revenue, cost, profit, profit_margin_pct
- Calendar:  order_month_name, order_month_num, order_month
- Geography: state (code), state_name, us_region, lat, lon
- Planning: budget (2024)
![Final Data Structure](Doc/Final%20Data%20Structure.png)

# 🎯 **Python Charts & Insights**
Here are some charts and insights related to dataset which provides deep details about the data set

## 🎯 **Monthly Sales Trend Over Time**

![Monthly Sales Trend](Doc/Monthly%20Sales%20Trend.jpg)

- Consistent sales cycle: $24M to $26M.
- Seasonal peaks: Late spring/early summer (May-June).
- Annual low: January.
- Notable outlier: Sharp revenue drop in early 2024.





