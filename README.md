# NYC-Property-Sales-Analytics

# NYC Property Sales Analysis (2016–2017)

A complete data analytics pipeline applied to the NYC Rolling Property 
Sales dataset — covering API ingestion, data cleaning, statistical 
analysis, visualization, and SQLite database export.

## Project Overview
Analyzed 84,548 residential property sale records across New York City's 
five boroughs between September 2016 and August 2017. After cleaning, 
56,566 valid residential records remained for analysis.

## Key Findings
- Sale price range: $1 – $620 million | Median: ~$620,000 | Mean: ~$1.17M
- Distribution is strongly right-skewed due to luxury properties
- Queens had the highest transaction volume; Manhattan had the highest median price
- Gross square footage had the strongest positive correlation with sale price
- Top neighborhoods: Upper East Side, Flushing, Upper West Side

## Tools Used
- Python (pandas, NumPy, Matplotlib) — cleaning, analysis, visualization
- SQLite — exported cleaned dataset into relational database
- opendatasets — Kaggle API integration
- Google Colab — development environment

## Pipeline Steps
1. API data import via Kaggle
2. Data cleaning — removed commercial properties, $0 sales, invalid ZIPs
3. Statistical analysis — distributions, correlations, outlier detection
4. Visualizations — 8 charts covering price, volume, geography, building type
5. SQLite export — 56,566 records written to nyc_property_sales.db

## Repository Structure
NYC-Property-Sales-Analytics/
├── NYC_Property_Sales_Analysis.ipynb
├── Project_Summary_Report.docx
└── README.md

## How to Run
1. Open notebook in Google Colab or Jupyter
2. Run cells top to bottom
3. Enter your Kaggle API credentials when prompted
4. Get your API key at kaggle.com/account

## Future Extensions
- Add year built or bedrooms for richer modeling
- Time-series analysis across multiple years
- Join with census or crime datasets
- Build predictive regression model for price estimation

## References
- NYC Rolling Property Sales — Kaggle / NYC Open Data
- pandas docs: pandas.pydata.org
- sqlite3 — Python Standard Library
