# Bank Customer Retention Dashboard

An interactive executive dashboard showing **who is leaving the bank, how much money leaves with them, and where the retention team should focus.**

### 👉 [Open the live dashboard](https://shanmukha-bhimireddy.github.io/bank-retention-dashboard/)

**Tools:** Plotly.js · HTML/CSS/JavaScript · GitHub Pages

## What it does
- **Filters** by country, gender and member status. Every KPI, chart, table and insight updates instantly.
- **KPI tiles:** customers, churn rate, balance lost, and the share of churn captured by a high-risk flag.
- **Charts:** churn by age band, by number of products, by country; balance lost by country; a country × age heatmap.
- **Table view** of the top-risk segments, plus an auto-generated "What to do" insight for the current selection.
- Hover tooltips on every chart, light/dark mode, and a mobile-friendly layout.

## Key insights (all customers)
| KPI | Value |
|---|---|
| Churn rate | **20.4%** (2,037 of 10,000 customers) |
| Balance lost | **$185.6M** |
| Riskiest segment | **Germany, age 50–59: 70% churn** |
| High-risk flag | **12% of customers → 42% of churn** |

- Germany churns at **32%**, about twice France and Spain, and accounts for **$98M** of lost balances.
- Customers with **2 products churn at 7.6%**; those with **3–4 products churn at 83–100%**.
- Churn climbs steeply after age 40 and peaks at **56% for ages 50–59**.

Companion SQL analysis: [bank-customer-churn-sql](https://github.com/shanmukha-bhimireddy/bank-customer-churn-sql)

## How it's built
`index.html` loads `data/Churn_Modelling.csv` in the browser, and all filtering and aggregation happens client-side, with no server or build step. GitHub Pages hosts it for free.

To run locally:
```bash
python -m http.server 8000
# then open http://localhost:8000
```

## Data
Public "Bank Customer Churn" dataset: 10,000 retail bank customers (France, Germany, Spain) with demographics, balances, product holdings, activity status and churn flag.

---
*Built by Shanmukha Sai Reddy Bhimireddy — Data / Business Analyst. Public data only.*
