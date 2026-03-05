# Manufacturers Sales Market Share Analytics

## An interactive Power BI dashboard analysing manufacturer-level sales performance, regional distribution, product category breakdown, and competitive market share trends over time.

# 📑 Table of Contents

- 📌 Project Overview
- ⚙️ Tools & Dependencies
- 🗄️ Data Sources & Data Model
- 🔍 Key Observations & Business Recommendations

 ## 📌 Project Overview
  
### This Power BI report is a manufacturer performance and market share dashboard built to help stakeholders understand:

- 💰 Sales revenue by manufacturer, product category, and region
- 🏆 Competitive market share positioning across manufacturers
- 📈 Year-over-Year (YOY) and rolling 12-month market share trends
- 🗺️ Geographic state-level sales distribution
- 📅 Time-based performance filtered by Year, Quarter, and Month

## ⚙️ Tools & Dependencies
| Tool | Version | Purpose |
|-----|---------|---------|
| PowerBi Desktop | Latest | Open, edit, and publish the report |
| Visual Studio Code | Latest | Inspect and edit raw JSON / TMDL files |
| Excel | Latest Version | To clean and edit raw data |

## 🗄️ Data Sources & Data Model
### Tables Overview
| Table | Type | Description | Key Columns |
|-------|------|-------------|-------------|
| SalesFact | Fact Table | Core transactional and market share data | Sales $, Units Market Share, Units Market Share YTD, Units Market Share SPLY, Units Market Share R12M, Unit Market Share YOY Change, Market Share SPLY YTD |
| Manufacturer | Dimension | Manufacturer names and attributes | Manufacturer |
| Product | Dimension | Product details and category groupings | Category |
| Geo | Dimension | Geographic hierarchy | State, Region |
| Date | Dimension | Full date hierarchy | Year, Quarter, Month |

## 🔍 Key Observations & Business Recommendations
The following recommendations are based on the data fields, KPIs, and visual structure of this report. These are actionable insights the business should consider to drive growth, improve competitiveness, and optimise performance.

| Area | Observation | Recommended Action | Priority |
|------|-------------|--------------------|----------|
| 1. Market Share Decline (YOY) | The Unit Market Share YOY Change measure tracks year-over-year shifts in competitive positioning. Any negative trend signals a manufacturer losing ground to competitors | Identify manufacturers with declining YOY market share and investigate root causes — pricing, distribution gaps, or product gaps. Develop targeted recovery plans with sales and marketing teams | 🔴 High |
| 2. Regional Sales Gaps | Geo.Region is used in the multi-dimensional column chart, revealing which regions contribute most and least to revenue. Some regions may be significantly underrepresented | Conduct a region-by-region gap analysis. Regions with low Sales $ relative to their population or market potential should be prioritised for new distribution partnerships or sales campaigns | 🔴 High |
| 3. Product Category Mix | Product Category is available in the multi-dimensional chart alongside manufacturer and region. Category-level profitability may differ significantly | Break down Sales $ and market share by Product.Category per manufacturer. Identify which categories are growing vs. declining and adjust inventory and production planning accordingly | 🟠 Medium |
| 4. Manufacturer Competitive Benchmarking | The line chart compares all manufacturers' market share trends, but there is no single "market leader" benchmark line | Add a calculated measure for the top-performing manufacturer's market share as a dynamic benchmark. All other manufacturers can then be compared against this ceiling to understand the gap they need to close| 🟡 Low |
| 5. Quarterly Trend Visibility | Date Quarter is available in the line chart but the primary filter is year-level only via the slicer | Add a Quarter slicer to allow users to drill into specific quarters for seasonal analysis. This is especially useful for manufacturers with strong Q4 or back-to-school sales cycles | 🟡 Low |

