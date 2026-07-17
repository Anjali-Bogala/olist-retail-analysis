# Olist Retail Analysis — Key Findings Summary

**Dataset:** 96,478 delivered orders · 96,096 unique customers
**Period:** January 2017 – August 2018
**Analyst:** Anjali Bogala

---

## Finding 1 — Delivery Timing Drives Satisfaction (HEADLINE)

**What:** Late delivery drops avg review score from 4.2★ to 2.26★

 Delivery Timing : Orders - Avg Review - Avg Order Value 

 Early (8-14 days before estimate) : 36,158 - 4.24★ - ₹115.69 |
 Very Early (15+ days) : 34,779 - 4.22★ - ₹124.52 
 Slightly Early (0-7 days) : 18,514 - 4.13★ - ₹114.13 
 Late (after estimate) :  6,381 - 2.26★ - ₹134.60 

**Key Insight:** 93.4% of orders arrive early , Olist uses a deliberate under-promise, over-deliver strategy. The 6.6% of late orders disproportionately affect high-spending customers (₹134.60 avg vs ₹115 for early orders).

**Recommendation:** Prioritise eliminating late deliveries for high-value product categories. Even a 50% reduction in late orders would recover ~₹4.76L in at-risk revenue from highest-value customers.

---

## Finding 2 — SP Volume Dilution Effect

**What:** SP has highest revenue but lowest avg item price (₹109)

**Root Cause Confirmed (verified with data):**
- Primary: Volume dilution — SP's 40,501 orders (42% of total) create a diverse basket that pulls the average down
- Secondary: Category mix — SP's top categories (bed/bath ₹91,health/beauty ₹110) are inherently lower-priced

**Opportunity:** PE (₹144), CE (₹154), PA (₹165) show high avg prices with lower volumes — potential underserved markets where customers buy higher-value items due to limited local retail access.

---

## Finding 3 — Watches & Gifts Revenue Efficiency

**What:** Comparable revenue to market leader with 37% fewer orders

| Category      | Orders | Revenue | Avg per Order |
| health_beauty | 8,647  | ₹12.3L  | ₹143          |
| watches_gifts | 5,495  | ₹11.6L  | ₹212          |

**Recommendation:** watches_gifts should be prioritised for seller
acquisition — higher revenue-per-transaction makes it more valuable
than order volume alone suggests.

---

## Finding 4 — RFM Customer Segments

**Total unique customers:** 96,096
**Segments identified:** 9

| Segment | Customers | Action |
| Champions | [X] | Reward + ask for referrals |
| Loyal Customers | [X] | Loyalty programs, upsell |
| Potential Loyalists | [X] | Targeted offers to convert |
| Recent Customers | [X] | Personalised follow-up |
| Promising | [X] | Engage before going cold |
| Need Attention | [X] | Re-engagement campaign |
| At Risk | [X] | Urgent win-back campaign |
| Cannot Lose Them | [X] | Immediate personal outreach |
| Lost | [X] | Low priority, minimal spend |

---

## Finding 5 — Revenue Growth Pattern

- Strong growth through 2017 with Nov 2017 as peak month
- Q4 consistently outperforms Q1 — seasonal pattern confirmed


---

## Data Quality Notes
- 2,963 non-delivered orders excluded (cancelled, processing, etc.)
- 610 products with missing category → filled as 'unknown'
- 1 order with no payment record found in raw data (left as NaN)
- 827 orders with no review score (customer never rated)
- All date columns converted from string to datetime