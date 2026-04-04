# Superstore Sales Dashboard

**Tools:** Power BI · DAX · Power Query · Excel
**Type:** Business Intelligence Dashboard
**Status:** Completed

---

## Overview

An end-to-end interactive Power BI dashboard built on the Sample Superstore dataset. Designed to give stakeholders a single view of regional sales performance, category trends, profit margins, and customer segments.

This project demonstrates real-world BI skills: data modelling, DAX measure writing, and dashboard storytelling.

---

## Dashboard features

- Regional sales breakdown with map visual
- Category and sub-category profitability analysis
- Year-over-year growth tracking
- Customer segment comparison (Consumer, Corporate, Home Office)
- KPI cards: Total Sales, Total Profit, Profit Margin %, Orders Count
- Dynamic slicers for Region, Category, and Date range

---

## Key DAX measures

```dax
Total Sales = SUM(Orders[Sales])

Profit Margin % = DIVIDE(SUM(Orders[Profit]), SUM(Orders[Sales]), 0)

YoY Growth % = 
DIVIDE(
    [Total Sales] - CALCULATE([Total Sales], SAMEPERIODLASTYEAR('Date'[Date])),
    CALCULATE([Total Sales], SAMEPERIODLASTYEAR('Date'[Date])),
    0
)
```

---

## How to open

1. Download the `.pbix` file from this repo
2. Open with [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free)
3. Use the slicers on each page to explore the data

---

## Key insights from the data

- Technology category drives the highest revenue but Furniture has the lowest margins
- The West region consistently outperforms other regions
- Same-day shipping has a significantly lower profit margin vs Standard Class

---

## Tech stack

| Tool | Purpose |
|---|---|
| Power BI Desktop | Dashboard development |
| Power Query (M) | Data cleaning and transformation |
| DAX | KPI measures and calculated columns |
| Excel | Initial data exploration |

---

## Connect

**LinkedIn:** linkedin.com/in/yaseen-544b8332b
**Email:** yaseenbinzubair2004@gmail.com
