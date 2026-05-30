# 📊 Power BI Dashboard Structure — EV_SALES.pbix

## Overview
- **File:** EV_SALES.pbix
- **Pages:** 4
- **Total Visuals:** 12
- **Custom Visuals Used:** Risk Heatmap, Box & Whisker with Points
- **Data Source:** ev_market_2026.csv (2,000 rows, 24 columns)

---

## Page 1 — Sales & Market Share
| # | Visual Title | Chart Type | X / Category | Y / Values | Series |
|---|---|---|---|---|---|
| 1 | Brand vs Total Sales | Column Chart | Brand | Sum(Annual_sales_units) | — |
| 2 | Market Segment Share | Donut Chart | Market_segment | Sum(Annual_sales_units) | — |
| 3 | Sales Growth Over Years | Line Chart | Year | Sum(Annual_sales_units) | — |

## Page 2 — Pricing & Value Analysis
| # | Visual Title | Chart Type | X / Category | Y / Values | Series |
|---|---|---|---|---|---|
| 1 | Price vs Range | Scatter Chart | Sum(Price_usd) | Sum(Range_miles) | Brand |
| 2 | Avg Price by Brand & Segment | Clustered Bar | Brand | Sum(Price_usd) | Market_segment |
| 3 | Price by Market Segment | Treemap | Market_segment | Sum(Price_usd) | — |

## Page 3 — Customer & Geographic Insights
| # | Visual Title | Chart Type | X / Category | Y / Values | Series / Notes |
|---|---|---|---|---|---|
| 1 | Top 10 Models by Customer Rating | Clustered Column | Model + Brand | Sum(Customer_rating) | Top 10 filter applied |
| 2 | Body Type by Country | Stacked Column | Country_of_origin | Count(Body_type) | Body_type |
| 3 | Brand × Segment Avg Price | Matrix / Pivot | Brand (rows) | Avg(Price_usd) | Market_segment (cols) |

## Page 4 — Technology Insights
| # | Visual Title | Chart Type | X / Category | Y / Values | Y2 / Line |
|---|---|---|---|---|---|
| 1 | Autopilot Level by Brand | Clustered Bar | Brand | Count(Autopilot_level) | — |
| 2 | Drive Type Distribution | Pie Chart | Drive_type | Count(Drive_type) | — |
| 3 | Range vs Charging Speed | Line & Column Combo | Brand | Avg(Range_miles) | Sum(Charging_speed_kw) |

---

## DAX / Aggregations Used
| Measure | Aggregation | Column |
|---|---|---|
| Total Sales | SUM | Annual_sales_units |
| Avg Price | AVERAGE | Price_usd |
| Total Price | SUM | Price_usd |
| Avg Range | AVERAGE | Range_miles |
| Total Charging Speed | SUM | Charging_speed_kw |
| Customer Rating | SUM | Customer_rating |
| Autopilot Count | COUNT NON NULL | Autopilot_level |
| Drive Type Count | COUNT NON NULL | Drive_type |
| Body Type Count | COUNT NON NULL | Body_type |
