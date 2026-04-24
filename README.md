# Real Estate Property Management Dashboard

## Table of Contents
- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Key Insights and Results](#key-insights-and-results)
- [Recommendations](#recommendations)
- [Limitations](#limitations)
- [How to Open](#how-to-open)

## Project Overview
Built a 3-page interactive Power BI dashboard on 21,613 housing records 
using a star schema data model (1 fact table + 5 dimension tables). The 
dashboard enables property managers and investors to filter by location, 
year built, and renovation year to analyse property condition, bedroom 
distribution, renovation patterns, and geographic hotspots for 
strategic decision-making.

## Data Sources
- **Dataset:** King County House Sales (modified for practice)
- **Source:** Kaggle — House Sales in King County, USA
- **Size:** 21,613 rows × 20 columns
- **Coverage:** 6 locations, properties built 1900–2015
- **Renovated properties:** 10,360 out of 21,613 (47.9%)

## Tools
- Power BI Desktop – Dashboard development and interactive visualisation
- DAX – Calculated columns and custom measures
- Power Query – Data cleaning and transformation
- Excel (.xlsx) – Source data format
- Star Schema – Data modelling (1 fact table + 5 dimension tables)

## Key Insights and Results
- 21,613 total properties analysed across 6 locations
- 3-bedroom homes are the most common segment — 9,824 properties (45.5%)
- Only 163 of 21,613 properties (0.75%) have waterfront access — 
  niche but high-value market segment
- 10,360 properties (47.9%) have been renovated at some point
- Over 52% of properties have never been renovated — 
  significant value-add investment opportunity
- Properties with 5–6 bedrooms are rare — less than 4% of total stock
- Single-floor homes dominate the market, followed by 2-floor properties

## Recommendations
- Focus investment on 3-bedroom properties — highest demand segment 
  at 45.5% of total stock
- Waterfront properties (0.75%) represent a niche premium segment — 
  worth tracking separately for pricing strategy
- Over 52% of properties have never been renovated — strong opportunity 
  for value-add investment and resale
- Properties in poor condition can be targeted for renovation given the 
  strong condition-to-price relationship visible in the dashboard
- Use year built filter to identify aging stock that may need 
  maintenance prioritisation

## Limitations
- Location labels (Arizona, California etc.) are modified from the 
  original King County, Washington dataset — geographic analysis 
  should be treated as illustrative only
- Condition column is numeric (0/1/2) in raw data — mapped to 
  Good/Very Good/Bad in the dashboard for readability
- Dataset is static — dashboard does not refresh with live market data
- Price data is from 2014–2015 and in USD — not reflective of 
  current market values
- No rental yield or ROI data available — investment return 
  analysis is not possible with this dataset

## How to Open

1. Download and install Power BI Desktop (free)
https://powerbi.microsoft.com/desktop

2. Clone the repository
git clone https://github.com/madhubandi533/real-estate-powerbi-dashboard.git

3. Open the dashboard
File → Open → dashboard/Real_estate.pbix

4. Update the data source path if prompted
   - Click `Transform Data`
   - Update file path to point to `data/Housing_dataset.xlsx`

5. Explore the dashboard
   - Use slicers on each page to filter by location, 
     year built, and renovation year
