# End-to-End Sales Performance & Customer Analytics

A complete sales analytics solution built from raw regional transaction records. This project combines an exploratory data analysis (EDA) pipeline in Python with a 3-page interactive Power BI dashboard to evaluate top-line growth, channel profitability, regional penetration, and customer spending tiers.

---

## 📌 Project Overview

The objective of this project is to analyze 64,000+ transaction records spanning 2014 to 2018 to uncover revenue drivers and operational bottlenecks. 

The workflow transitions from raw data auditing and feature engineering in Python to data modeling and executive reporting in Power BI:
1. **Python Data Pipeline & EDA:** Cleaned raw transactions, engineered profit and margin metrics, evaluated statistical distributions, mapped geospatial performance, and exported a standardized CSV.
2. **Power BI Modeling & Visualization:** Designed a star schema with time intelligence DAX metrics and built a 3-page interactive dashboard for executive review.

---

## 🛠️ Tech Stack & Libraries

* **Language & Core Libraries:** Python 3.x (Pandas, NumPy)
* **Data Visualization (Python):** Matplotlib, Seaborn, Plotly Express
* **Business Intelligence & Modeling:** Power BI Desktop, DAX, Power Query
* **Data Output:** Pre-processed CSV dataset

---

## 📊 Exploratory Data Analysis (EDA) Highlights

The Python notebook performs a line-by-line evaluation of sales performance across 15 analytical sections:

* **Feature Engineering:** Calculated gross revenue, total order cost, net profit, and percentage profit margins per transaction.
* **Channel Mix:** Identified Wholesale as the primary volume driver (54% of sales), while maintaining uniform profit margins across Export (37.93%), Distributor (37.56%), and Wholesale (37.09%).
* **Regional Dominance:** California led all market sales at ~$230M across 7,500+ orders, with revenue closely correlating to order volume across top states.
* **Geospatial & Bivariate Mapping:** Built interactive Plotly choropleth maps and Seaborn box plots to analyze price spreads ($1,000–$3,800) and flag promotional giveaway outliers near $0–$100.
* **Multicollinearity Checks:** Constructed an annotated correlation matrix confirming a strong linear relationship between unit price, gross revenue (r = 0.91), and total cost (r = 0.94).

---

## 📈 Power BI Dashboard Architecture

The Power BI report is structured across three pages:

├── Page 1: Executive Overview & Trends
│   ├── Top-level KPI Cards (Total Revenue, Profit, Margin %, Orders, AOV)
│   ├── Monthly Revenue Rhythm & Profit Pulse Line Charts
│   └── Order Value Histogram & Unit Price vs. Margin Scatter Plots
│
├── Page 2: Product & Channel Performance
│   ├── Revenue Champions (Top Products by Revenue) & High-Margin Heroes
│   ├── Strategic Product Positioning (Revenue vs. Margin % Scatter)
│   └── Channel Revenue, Profit, and Efficiency Breakdown
│
└── Page 3: Geographic & Customer Insights
├── Top/Bottom 5 Customer Toggles (Revenue & Margin %)
├── State & Regional Revenue Performance
└── Interactive Regional Bubble Map

## 🔍 Key Business Insights

1. **Revenue Stability:** Monthly sales averaged $23M–$26.5M across 2014–2017, with a temporary dip to ~$21.2M in early 2017.
2. **Channel Expansion Opportunity:** Export accounts for only 15% of revenue despite matching domestic profit margins (~37–38%), presenting an international scaling target.
3. **Customer Value Drivers:** High customer lifetime value is driven by order frequency (60–90 orders) rather than isolated high-margin orders.

---

## 💡 Strategic Recommendations

* **Pricing Strategy:** Standardize promotional SKU logging ($0–$100) to prevent skewing baseline transaction averages.
* **Market Focus:** Increase distributor investment in secondary high-volume states (Illinois at $112M, Florida at $90M) while expanding international export marketing.
* **Inventory Alignment:** Align procurement schedules around seasonal volume peaks in May–June.

---