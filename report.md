# ShopSphere Analytics Report

## Analysis Objective
The goal of this project was to analyze the effectiveness of the e-commerce platform and find answers to key business questions: where the marketing budget is being spent, who the most valuable customers are, which product categories are truly profitable, and whether the new checkout page design contributed to sales growth.

## Data
The analysis is based on 5 CSV tables covering the period from 2022 to 2024. The dataset includes 3,000 customers, 12,274 orders, 26,068 order items, 250 products across 7 categories, and 216 marketing campaign records across 6 channels. Tables are connected via customer, order, and product IDs.

## Methodology
Data was prepared and aggregated using SQL (SQLite) with JOINs and subqueries. Further analysis was done in Python using pandas for data manipulation, scipy for statistical testing, and Prophet for revenue forecasting. The A/B test was evaluated using an independent samples t-test (ttest_ind). Visualizations were built in Tableau and matplotlib.

## Results
**Marketing.** Organic is the most efficient channel with an ROI of 702x at a budget of only $20K. Paid Search has the largest budget ($450K) but the lowest ROI (32x) — a clear sign of poor allocation. When looking at customer lifetime value by channel, Influencer leads with an average LTV of $1,985, followed by Referral ($1,791). Paid Search brings in the lowest-value customers at $648 LTV — poor on both ROI and customer quality. ROI and LTV tell different stories, and both metrics matter.

**Categories.** Electronics generates the highest revenue (~$2.9M) but has the lowest margin (12%) and the highest return rate (17.8%) — it creates an illusion of volume. Beauty has the highest margin (~55%) with a moderate return rate, making it the most profitable category per dollar sold. Sports has the lowest return rate (9%) and a solid margin of 30%.

**Customers.** The top 5% of customers (150 people) generate 35% of total revenue ($1.2M), spending 7x more than the average buyer. Most of them came through Influencer or Organic channels. Customers who buy mostly with discounts (average discount >20%) place twice as many orders on average (4.5 vs 2.2), which suggests they are price-sensitive but loyal when incentivized.

**A/B Test.** The new checkout design (variant B) showed a slightly higher average order value ($287 vs $282), but the difference was not statistically significant (p = 0.51). Breaking down by customer type, new customers in group B spent $283 vs $263 in group A — a promising trend, but still not significant (p = 0.71). The experiment did not produce conclusive results.

**Forecast.** A Prophet model trained on 2022–2024 monthly revenue predicts a December 2025 peak of +/- $697K, consistent with prior holiday seasonality. Revenue is expected to drop sharply in January 2025 (~$148K) before recovering through the year.

## Recommendations
The most impactful thing would be realocating Paid Search budget by 40-50% and moving that money to a Organic, Refferal and Email - channels that bring better returns and higher-quality customers. Beauty and Sports are also worth investing in more: both have strong margins and few returns, but are currently underdeveloped.

The top 5% of customers bring in 35% of all revenue, so losing even a few of them hurts. A simple VIP program — early access to new products, personal service — would help keep them. For customers who mostly buy on discounts, a reward system like "get a bonus on your 5th order" works better than constant sales, because it builds loyalty without cutting into profit.

Before making any decision about the new checkout design, the A/B test should be run again with more users and over a longer period. The current results are too inconclusive to act on.

## Limitations
The A/B test ran on a small sample for a short time, which is why the results were inconclusive. The dataset is fictional, so real-world data would likely be messier. The forecast is based on past patterns and won't be accurate if market conditions change.
