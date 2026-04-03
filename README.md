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

## 🎯 **Top 10 Products by Revenue**

![Top 10 Products By Revenue](Doc/Top%2010%20Products%20By%20Revenue.jpg)

- Revenue leaders: Products 26 & 25 dominate.
- Mid-range: Products 5, 13, 14, 15 show similar revenue.
- Bottom cluster: Products 1, 2, 3, 4 have the lowest revenue.
- Strategy: Grow mid-tier, improve lower performers.

## 🎯 **Top 10 Products by Average Profit Margin**

![Top 10 Products by Avg Profit Margin](Doc/Top%2010%20Products%20by%20Avg%20Profit%20Margin.jpg)

- Top: Products 18 & 28 lead at ~$8.1–8.4K.
-Next tier: Products 5, 11, 12 & 26 at ~$7.5–7.8K.
-Entry‑level: Products 1, 4, 16 & 21 around $7.3K.
-Takeaway: Top 10 all exceed $7.3K—consistent high margins.

## 🎯 **Sales by Channel**

![Sales By Channel](Doc/Sales%20By%20Channel.jpg)

- Wholesale dominates: Generates the majority of total sales at 54.1%.
- Distributor is significant: Contributes a substantial 31.3% to total sales.
- Export is a smaller portion: Accounts for 14.6% of the total sales.

- 
## 🎯 **Total Sales by US Region**

![Total Sales by US Regionl](Doc/Total%20Sales%20by%20US%20Region.jpg)

•West: Highest sales, strong market influence.
•South: Major sales contributor, key market area.
•Midwest: Steady sales performance, moderate market size.
•Northeast: Lowest sales, suggests need for deeper market understanding.

## 🎯 **Average Order Value (AOV) Distribution**

![Average Order Value](Doc/Averagel%20Orderl%20Value.jpg)

•Low average order values are frequent.
•Distribution is right-skewed (long tail of high-value orders).
•Multiple order value clusters exist.
•Higher order values are less common.

## 🎯 **Top State Performance: Revenue vs. Orders**

![Top 10 State By Revenue](Doc/Top%2010%20State%20By%20Revenue.jpg)

![Top 10 State By Order](Doc/Top%2010%20State%20By%20Order.jpg)

•California tops revenue & orders.
•IL, FL, TX: High in both.
•Revenue & orders linked.
•Other top states: Lower contribution.

## 🎯 **Top and Bottom 10 Customers by Revenue**

![Top 10 & Bottom 10 Customer By Revenue](Doc/Top%2010%20& Bottom%2010%20Customer%20By%20Revenue.jpg)

•Aibox Company leads significantly as the top revenue generator.
•Bottom 10 customers generate substantially less revenue (around $4-5M).
•Revenue concentration: Top customers drive a disproportionate share.
•Large gap: Exists between the revenue of top and bottom tier customers.

## 🎯 **Customer Segmentation: Revenue vs. Profit Margin**
![Revenue vs. Profit Margin](Doc/Revenue%20vs.%20Profit%20Margin.jpg)

•Those Uniform 35–40 % margins confirm strong, consistent pricing and cost control.
•>$10 M clients with <36 % margins reveal discounting hotspots—re evaluate large‑account terms.
•$6–9 M clients with >40 % margins are high‑value candidates for targeted upsell.



## 🎯 **Correlation Heatmap of Numeric Features**

![Numeric Features](Doc/Numeric%20Features.jpg)

•Unit price is the primary driver, showing very strong correlations with cost (0.94), revenue (0.91) and profit (0.79).
•Revenue & profit maintain a high link (0.87), underscoring direct profitability gains.
•Quantity’s impact is minimal (≤ 0.34 vs. financials), indicating volume plays a secondary role.
•Cost vs. profit correlation (0.58) is moderate, suggesting margin improvement focus should center on pricing.











