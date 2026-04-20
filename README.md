# Mobile Sales Dashboard

A comprehensive Power BI dashboard for analyzing mobile unit sales, performance trends, and market insights across regions and payment methods.

## Overview

This dashboard provides real-time visibility into mobile sales operations with interactive filtering and detailed breakdowns by model, payment method, brand, and geography.

---

## Dashboard Pages

### 1. Mobile Unit Sales Dashboard

![Mobile Unit Sales Dashboard](images/Screenshot%202026-04-20%20at%2016.35.22.png)

**Main KPIs:**
- Total Sales: **195M**
- Total Units: **5K**
- Total Transactions: **973**
- Average Price: **40.05K**

**Visualizations:**
- **Year-over-Year Comparison** — Current year (light blue) vs. same period last year (dark blue) side-by-side bars
- **Daily Breakdown Table** — Detailed transaction-level data with Year, Quarter, Month, Day, Sales, and YoY comparison columns
- **Monthly Sales Trend** — Bar chart showing quarterly (Q1-Q4) and monthly performance patterns
- **Daily Sales Detail** — Granular day-by-day sales data for January with 31 days visible

**Interactive Filters:**
- Mobile Model (All/specific)
- Payment Method (All/specific)
- Year (2024 default)
- Monthly selector on left sidebar

---

### 2. MTD Report (Month-to-Date Analysis)

![MTD Report Dashboard](images/Screenshot%202026-04-20%20at%2016.35.50.png)

**Current KPIs:**
- Total Sales: **769M** (MTD)
- Total Units: **19K**
- Total Transactions: **4K**
- Average Price: **40.11K**

**Key Visualizations:**

**Quantity Trends**
- Monthly quantity line chart showing seasonal patterns (Jan: 1672 → Dec: 1609 units)
- Peak sales in March (1696 units) and April (1700 units)

**Customer Satisfaction**
- **Customer Ratings Distribution** — 100% rated as "Best", 28% as "Average", with 852 "Poor" ratings
- Clear visual breakdown of satisfaction metrics

**Payment Methods**
- **Pie Chart** — UPI dominates (26.36%), followed by Debit Card (24.72%), Credit Card (24.69%), and Cash (24.22%)
- Equal distribution across payment types

**Geographic Analysis**
- **Interactive Map** — Sales coverage across 14 Indian cities:
  - North: Ludhiana, Delhi, Lucknow, Gurgaon, Patna
  - Central: Indore, Kanpur, Ranchi
  - South: Bangalore, Hyderabad, Chennai, Coimbatore, Kolkata
  - West: Mumbai, Bhopal
- Bubble markers showing sales intensity by location

**Brand Performance**
- **Top Brands by Sales:**
  - Xiaomi: 143.7B sales, 74 transactions
  - Vivo: 150.1B sales, 76 transactions
  - OnePlus: 153.7B sales, 76 transactions
  - Samsung: 160.3B sales, 77 transactions

**Mobile Models**
- iPhone SE, OnePlus Nord, Galaxy Note 20 among top sellers
- Horizontal bar chart showing sales volume by model

**Day-of-Week Analysis**
- Sales pattern across 7 days
- Monday shows highest sales (26M), declining through the week
- Weekend dip visible in data

**Interactive Filters:**
- Mobile Model dropdown
- Payment Method dropdown
- Brand dropdown
- Monthly selector on left sidebar

---

### 3. MTD by Year, Quarter and Month

![MTD Trend Analysis](images/Screenshot%202026-04-20%20at%2016.36.05.png)

**Purpose:** Track month-to-date trend progression throughout 2024

**Key Insights:**
- **Peak Performance** — March 2024: 23.9M (highest MTD)
- **Trend Pattern** — Strong start (21.9M in Jan), dips Feb-March, recovers in spring
- **Q2 Peak** — April-May shows strong performance (21.7M-23.9M)
- **Decline Trend** — Gradual decrease from July onwards (21.3M → 6.3M)
- **Seasonal Drop** — Significant decline post-September

**Metrics Displayed:**
- Continuous line chart tracking MTD through all months
- Clear labeling of peaks and valleys
- Year context showing Jan 2024 through Sep 2024+

**Use Cases:**
- Identify best performing months
- Forecast seasonal trends
- Monitor YTD progress
- Plan inventory and staffing

---

## What's Inside

- **Mobile Units Sales Dashboard.pbix.zip** — Power BI dashboard file with 3 interactive pages and all visualizations
- **Mobile Sales Data.xlsx** — Raw sales data (Year, Quarter, Month, Day, Total_Sales, Quantity, Payment Method, Brand, Mobile Model, Customer Ratings, Transaction ID, Location)

---

## Getting Started

### Requirements
- Microsoft Power BI Desktop (free or Pro version)
- Windows, macOS, or Power BI Service access
- Excel 2016 or later (optional, for data editing)

### Setup

1. Extract `Mobile Units Sales Dashboard.pbix.zip` to a folder
2. Open the `.pbix` file in Power BI Desktop
3. The dashboard connects to `Mobile Sales Data.xlsx` automatically
4. Verify the Excel file is in the same directory as the Power BI file
5. Click **Refresh** if you see a data connection prompt

### Using the Dashboard

**Navigating Pages:**
- Use the left sidebar buttons to switch between:
  - Mobile Unit Sales Dashboard (main overview)
  - MTD Report (detailed analysis)
  - MTD by Year, Quarter and Month (trends)

**Filtering Data:**
- **Dropdown Filters** (top of page) — Select specific Mobile Model, Payment Method, Brand, or Year
- **Month Selector** (left sidebar) — Click any month to focus on that period
- **All selections** — Click "All" to reset filters to full dataset

**Exploring Charts:**
- **Hover** over bars, lines, or map points to see exact values
- **Click** on map cities, brand names, or pie slices to cross-filter other visualizations
- **Scroll** through transaction tables for individual record details
- **Zoom** into specific areas by clicking and dragging on charts

---

## Data Management

### Updating Sales Data

1. Open `Mobile Sales Data.xlsx` in Excel
2. Locate the appropriate sheet (Sales, Transactions, Ratings, etc.)
3. Add or edit rows following the existing format:
   ```
   Year | Quarter | Month | Day | Total_Sales | Quantity | Payment_Method | Brand | Mobile_Model | Rating | Location
   2024 | Q1      | Jan   | 15  | 850000      | 25       | UPI            | Xiaomi| iPhone SE    | Best   | Mumbai
   ```
4. Save the file
5. Return to Power BI and click **Home > Refresh** to pull the latest data
6. All charts and metrics update automatically

### Adding New Locations

If adding new cities to the map:
1. Add location names and coordinates to the Excel data
2. Ensure Location column matches exactly (case-sensitive)
3. Refresh in Power BI
4. Map will automatically include new cities

### Handling Large Data

For performance with large datasets:
- Consider archiving historical data to a separate sheet
- Filter to current year/quarter when not needed for trend analysis
- Use incremental data refresh in Power BI Service

---

## Key Features

✓ **Real-Time Filtering** — Instantly see data by model, payment method, brand, date  
✓ **Geographic Insights** — Map visualization covering 14+ Indian cities  
✓ **Trend Analysis** — Identify seasonal patterns and growth/decline periods  
✓ **Customer Satisfaction** — Track ratings and transaction quality  
✓ **Payment Analytics** — Compare performance across UPI, cards, and cash  
✓ **Brand Comparison** — See which brands drive revenue and volume  
✓ **YoY Tracking** — Compare current year to previous year performance  
✓ **Transaction Detail** — Drill down to individual sales records

---

## Troubleshooting

| Issue | Solution |
|-------|----------|
| **Charts show no data** | Click **Home > Refresh** to reload data from Excel |
| **Data connection error** | Verify `Mobile Sales Data.xlsx` is in the same folder as `.pbix` file; check file path in **Transform Data > Data Source Settings** |
| **Filters not working** | Reset filters by clicking the filter icon and selecting **Clear All**; ensure filter values exist in your data |
| **Map not showing locations** | Verify location names in Excel match map city names exactly (case-sensitive) |
| **Slow performance** | Reduce date range, filter to single brand/model, or limit to current quarter |
| **Missing month data** | Check that month names follow format: January, February, etc. (not abbreviated) |

---

## Tips for Best Results

- **Monthly Updates** — Refresh data on the 1st of each month with latest sales figures
- **Backup Data** — Keep a copy of Excel file before major updates
- **Filter Logic** — Use "All" filters to see full dataset; narrow down for specific analysis
- **Presentation Mode** — Press F5 in Power BI for full-screen dashboard view in presentations
- **Export Reports** — Right-click any chart and select "Export Data" for sharing specific metrics

---

## Support & Questions

For questions about:
- **Dashboard Usage** — Review the "Using the Dashboard" section above
- **Data Updates** — See "Data Management" section
- **Building New Charts** — Open Power BI and review existing relationships in the Model view
- **Performance Issues** — Check the "Troubleshooting" table

To modify dashboard structure or add new pages, edit the `.pbix` file directly in Power BI Desktop.
