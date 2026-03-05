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






