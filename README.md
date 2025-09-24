
Data Preparation

- Imported `dataFB.xlsx` into Power BI and renamed the query to `Ads`.
- Created clean `Date` column from `reporting_start`.
- Set correct data types for impressions, clicks, spend, conversions, approved conversions.
- Renamed columns (spend, conversions, approved_conversions).
- Replaced nulls in numeric columns with 0.
- Removed duplicates based on `ad_id` and `Date`.
- Added `AgeGroup` column and unpivoted interest columns for easier analysis.

Data Model

- Created a separate `Date` table and linked it to `Ads[Date]`.
- Marked the `Date` table as a proper date table.

Dashboard Pages

- Executive Summary – Spend, Impressions, Clicks, CTR, ROAS cards and trend charts with slicers.
- Top Ads – Top-performing ads by clicks or conversions with Top N filter.
- Audience – Age group CTR, Gender distribution, Interests analysis.
- ROI & Conversions – Campaign metrics, CPA, ROAS with conditional formatting.
- Ad Drillthrough – Detailed per-ad page accessible from right-click drillthrough.

How to Use

1. Place raw Facebook Ads data in `ads-project/data/raw/dataFB.xlsx`.
2. Open the `.pbix` file in Power BI Desktop.
3. Click **Refresh** to load and transform data.
4. Interact with visuals, slicers and drillthrough pages to explore performance.
