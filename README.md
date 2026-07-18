# Olist Retail Sales Intelligence Platform

## Project Overview
End-to-end data analysis of the Brazilian Olist e-commerce platform(100,000+ orders, 9 related tables, 2016–2018). Built to simulate a
real industry analytics engagement — from raw messy data through SQL analysis, Python EDA, customer segmentation, to executive insights.

**Business Question:** What drives customer satisfaction and revenue on the Olist platform — and where are the biggest opportunities?

## Key Findings

### 1. Late Delivery Cuts Satisfaction Nearly in Half
- 93.4% of orders arrive BEFORE the estimated delivery date
- On-time/early orders average 4.13–4.24 ★
- Late orders average just 2.26 ★ — a 1.87-star drop
- Late orders paradoxically have the HIGHEST avg order value (₹134 vs ₹115 for early) — meaning the worst experience falls on
  the best customers

### 2. SP Volume Dilution Effect
- São Paulo (SP) generates the highest total revenue but has the LOWEST average item price (₹109 vs national avg ₹120+)
- Root cause confirmed: volume dilution — 42% of all orders come from SP, diluting the average with diverse everyday purchases
- Smaller remote states (PA, CE, PE) show avg prices of ₹154–165,signalling high-intent buyers in underserved markets

### 3. Hidden Revenue Efficiency in Watches & Gifts
- health_beauty leads in order volume (8,647 orders)
- watches_gifts generates comparable revenue (₹11.6L vs ₹12.3L) with 37% fewer orders — avg order value ₹212 vs ₹143
- Revenue-per-transaction analysis reveals watches_gifts as a priority category for seller acquisition

### 4. RFM Customer Segmentation
- 96,096 unique customers segmented into 9 behavioural groups
- Champions and Loyal Customers drive disproportionate revenue
- "Cannot Lose Them" segment: high-value customers going silent
  — immediate win-back action recommended
- "Need Attention" is the largest segment (28,899 customers) — 
  drifting buyers who need re-engagement before permanently churning
- "At Risk" segment (13,192 customers, avg spend ₹214) is highest 
  priority for win-back campaigns
- "Lost" segment: lowest priority for marketing spend

### 5. Revenue Growth Pattern
- Strong MoM growth through 2017, peak in Nov 2017
- Seasonal patterns visible — Q4 consistently outperforms Q1
- Cumulative revenue curve shows accelerating growth in H2 2017

## Project Structure
```
olist-retail-analysis/
├── data/
│   └── cleaned/              ← analysis-ready CSVs
├── notebooks/
│   ├── 01_data_understanding ← load + audit all 9 tables
│   ├── 02_schema_mapping     ← ERD + join verification
│   ├── 03_data_cleaning      ← pipeline: dates, NULLs, master table
│   ├── 04_sql_setup          ← GROUP BY, HAVING, business queries
│   ├── 05_advanced_sql       ← JOINs, subqueries, window functions
│   ├── 06_eda_charts         ← 4 business visualisations
│   └── 07_rfm_segmentation   ← RFM scoring + customer personas
├── reports/
│   ├── findings_summary.md   ← executive summary CSV
│   ├── rfm_segment_summary   ← segment breakdown C │   ├── olist_dashboard.pdf   ← Power BI dashboard export
│   └── dashboard_screenshot  ← dashboard preview image
│   └── charts (*.png)        ← 5 exported visualisations
└── README.md
```

## Tech Stack
| Tool | Purpose |
|---|---|
| Python 3.12 | Data cleaning, analysis, visualisation |
| pandas | Data manipulation and transformation |
| SQLite + SQL | Business queries, JOINs, window functions |
| matplotlib / seaborn | EDA charts |
| Power BI | Interactive dashboard |
| Git / GitHub | Version control, portfolio hosting |

## Dataset
**Brazilian E-Commerce Public Dataset by Olist** (Kaggle)
- 99,441 orders · 9 related tables · 2016–2018
- Tables: orders, customers, products, order_items, payments,
  reviews, sellers, geolocation, category_translation

## Author
**Anjali Bogala** — Data Science Portfolio Project
GitHub: [Anjali-Bogala](https://github.com/Anjali-Bogala)
