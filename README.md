# Marketing Campaign Performance Dashboard (Excel)

Interactive Excel dashboard analyzing 500 marketing campaigns across 5 channels and 4 regions: return on ad spend, cost efficiency and budget control.

![Dashboard](screenshots/01_dashboard_full.png)

## Business problem
Marketing teams need to know which channels and regions turn ad spend into revenue. This project converts raw campaign records into a dashboard that tracks profitability, efficiency and ROAS, and highlights underperforming channels.

## Key results
| Metric | Value |
|---|---|
| Total spend | 3,132,508 USD |
| Total revenue | 6,552,948 USD |
| Total profit | 3,420,440 USD |
| Overall ROAS | 2.09x |
| CTR | 2.91% |
| CPA | 16.98 USD |

## Key insights
1. Twitter has the largest budget (21.1%) but the lowest ROAS (1.83x vs Instagram 2.29x).
2. Facebook ROAS ranges from 2.74x in North to 1.64x in East, so results depend on region.
3. Facebook has the best CTR (3.17%) but converts 9.74% of clicks vs Instagram 11.13%.
4. 157 of 500 campaigns overspent their budget, although total spend is 5.4% under budget.
5. 158 campaigns (31.6%) earned less than they spent, a net loss of 430,111 USD.
6. West has the cheapest clicks (1.59 USD) and the highest profit.

## Recommendations
- Move part of Twitter's budget to Instagram and Facebook (modeled 10% shift: about +30,487 USD revenue, an upper estimate).
- Set budgets per channel-and-region pair, not per channel.
- Add an alert at 100% budget utilization and review loss-making campaigns (ROAS below 1).

## Workflow
1. Cleaned the data in Power Query (types, trimming, duplicate check).
2. Built calculated columns: CTR, CPC, CPA, ROAS, Profit, Profit Margin, Conversion Rate, Budget Utilization, Performance Tier.
3. Built 10 PivotTables with weighted calculated fields.
4. Designed the dashboard with 7 KPI cards, 5 charts, slicers and a date timeline.

## Screenshots
![Filtered view](screenshots/02_dashboard_facebook_filter.png)
![Power Query steps](screenshots/03_power_query_steps.png)
![Pivot tables](screenshots/04_pivot_tables.png)

## Files
| File | Purpose |
|---|---|
| Marketing_Campaign_Dashboard.xlsx | Final workbook (download to use the slicers) |
| data/Marketing_Campaign_Data_ORIGINAL.xlsx | Untouched raw data |
| screenshots/ | Images of the dashboard and workflow |

## Limitations
About 6 months of data; December and June are partial months; no cost-of-goods data.
