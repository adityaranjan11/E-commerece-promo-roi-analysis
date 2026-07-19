# E-Commerce Promo Campaign ROI Analysis
**Tech Stack:** Python (Pandas, Matplotlib), SQL (DuckDB Database Engine)

## Executive Summary
This project evaluates the financial impact of a 30-day promotional marketing campaign executed in February 2026. While marketing campaigns aim to drive order volume, this analysis investigates whether the heavy discounting structure ultimately harmed net profitability and customer retention.

## Key Insights & Business Impact
* **The Revenue Trap:** In February, the promotional campaign successfully drove transaction volume, but giving out over **$50,776** in discounts caused **Net Revenue to plummet by over $73,000** compared to the January baseline.
* **Margin Cannibalization:** Average Order Value (AOV) dropped severely from **$174.16** down to **$143.27** during the campaign, proving that customers were buying cheaper items or relying heavily on steep discounts.
* **Retention Deficit:** Customers acquired through the massive February discount codes showed a **15% lower Month-1 retention rate** than organic customers acquired in January, indicating the promo drew transactional bargain-hunters rather than long-term loyal users.

## Project Architecture & Methodology
1. **Data Engineering & ETL (Python):** Ingested raw transactional records, handled duplicate transactions, isolated returns, mapped complex discount structures, and imputed missing guest user accounts.
2. **Analytical Layer (SQL):** Loaded the structured dataset into a high-performance analytical DuckDB database. Wrote advanced Common Table Expressions (CTEs) and window functions to compute monthly metrics and cohort retention percentages.
3. **Data Visualization:** Built visual frameworks in Python to contrast gross transaction metrics against realized post-discount revenue.
