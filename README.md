# vivekvishwakarma_bitsom_ba_2511306_part4_tableau_dashboard

# Part 4: Executive Dashboard & Data Storytelling

## Business Problem Summary
The retail leadership team requires an executive-level diagnostic tool to monitor organizational health. This project transforms raw operational data into a unified dashboard that identifies revenue drivers, margin bleed, logistical bottlenecks, and optimal discounting strategies.

## UI/UX Engineering & Design Philosophy
This dashboard abandons standard spreadsheet-style layouts in favor of a modern, SaaS web-application aesthetic. 
- **Dark Mode Architecture:** Utilizes a `#121212` background with `#232730` padded layout containers to reduce eye strain and establish a sleek, card-based hierarchy.
- **Data-Ink Optimization:** All native gridlines, axis rulers, and unnecessary borders were stripped to maximize signal-to-noise ratio.
- **Cognitive Ergonomics:** Interactive filters are grouped into a unified, collapsible sidebar panel (dropdowns) rather than scattered across the screen, ensuring a seamless executive user experience.

## Dataset Description
- **Source:** `dashboard_sales_data.xlsx`
- **Scope:** Granular, order-level data encompassing sales, profit, categorical hierarchy, geographic locations, and shipping logistics.

## Calculated Fields Created
1. **Profit Margin:** `SUM([profit]) / SUM([sales])`
2. **Cost:** `[sales] - [profit]`
3. **Average Order Value (AOV):** `SUM([sales]) / COUNTD([order_id])`
4. **Return Rate:** `SUM([return_flag]) / COUNT([order_id])`
5. **Shipping Delay Bucket:** Categorizes `delivery_days` into Fast (0-3), Standard (4-5), and Delayed (6+).

## Dashboard Components & Interactions
- **Visuals:** Top KPI Banner, Sales Trend Area Chart, Regional Performance Map, Category Profitability Bar, Discount Scatter Plot, Segment Donut Chart.
- **Interactions:** The dashboard utilizes unified action filters—selecting a specific Region, Category, or Date range from the left sidebar instantly updates all supplementary charts and KPI cards to reflect that specific segment's performance.

## Key Business Insights
Top-line sales growth is masking severe margin erosion caused by aggressive discounting (specifically discounts exceeding 20%). While the Corporate segment and Office Supplies category generate robust profits, heavily discounted Furniture in specific regions acts as a loss-leader. Leadership must cap discounts at 15% and reallocate resources toward high-margin B2B acquisition.

## Screenshots Included
- `full_dashboard.png`
- `sales_trend_view.png`
- `regional_performance_view.png`
- `category_profitability_view.png`
- `filter_interaction_view.png`
