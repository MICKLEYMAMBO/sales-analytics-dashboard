SalesRite Store Performance Dashboard
An Excel-based sales analytics dashboard built on a 4-year, ~10,000-row retail dataset. The workbook takes raw order and returns data through a full data-quality assessment, cleaning, relationship-building, and a live, filterable dashboard with KPIs, charts, and a written insight summary.


Overview
Dataset: SalesRite Store, 2022–2025 — 9,994 order line items (5,009 distinct orders), 296 returns, 4 regional managers
Total Sales: $2,297,200.86
Total Profit: $286,397.02 (12.47% margin)
Total Orders: 5,009 | Return Rate: 5.91%

Workbook Structure
Sheet
Purpose
Sales Dashboard

The main interactive dashboard — KPI cards, charts, and slicers
Insight Summary
Written narrative of findings and recommended actions
Pivot source
Supporting pivot tables feeding the dashboard's charts
Orders
Cleaned order-level data (21 source columns + calculated fields)
Returns
Return records, matched back to Orders
Manager
Region-to-manager lookup table
Data Dictionary
Column-by-column definitions for every field in the workbook
Data Quality Report
Documented data-quality checks and cleaning actions taken
Data Quality Process
Before any analysis, the raw dataset went through a documented quality assessment (see the Data Quality Report sheet):

Checked for exact duplicate rows, missing values, inconsistent formatting, invalid/impossible values, and referential integrity between Orders, Returns, and Manager tables
Found the source data was largely clean: no missing values across all 21 columns, no exact duplicates, dates and numeric types already correct
Added calculated fields to support the analysis: Order Year, Order Quarter, Order Month, Order Month Name, a Manager lookup (via Region), a Returned flag (matched against the Returns table), and two distinct-count flag columns used to calculate order and return-rate totals without array formulas
Validated totals (sales, profit, row count) were unchanged before vs. after cleaning, and confirmed 100% of Returns records matched an Order ID
Dashboard Features
KPI Cards: Total Sales, Total Profit, Profit Margin %, Total Orders, Total Quantity Sold, Return Rate %
Charts:

Sales & Profit by Region
Sales & Profit by Manager
Sales by Category
Sales by Sub-Category
Sales Trend Over Time (Month/Year)
Top 10 Products by Profit
Return Rate by Manager
Slicers (interactive filters): Region, Category, Manager, Order Date (Year) — every KPI and chart updates live as filters are applied.
Key Insights
Sales grew every year from 2022 to 2025, a 51% increase overall ($484K → $733K)
Technology is the strongest category by margin (17.4%); Furniture is the weakest (2.5%), dragged down by structurally unprofitable Tables and Bookcases sub-categories
West region (Anna Andreadi) leads on both sales and margin; Central region (Kelly Williams) has the lowest margin of the four regions despite mid-pack sales volume
Return rate is a consistent 5.9% across regions, not concentrated in any one manager's territory
Full recommendations are documented in the Insight Summary sheet.

Skills Demonstrated
Data quality auditing and documented cleaning methodology
Formula-driven KPI and lookup logic (SUMIFS, SUMPRODUCT, INDEX/MATCH)
Pivot tables, pivot charts, and synchronized slicers
Dashboard design and data storytelling
Files
Sales_Dashboard_-_Mambo_Mickley.xlsx — the full workbook

Built by Mambo Mickley as part of an ongoing Business Intelligence & Data Analytics portfolio.