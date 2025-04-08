# Electricity Price Volatility Analysis (France – EPEX Spot)

## What I Did

- Collected hourly electricity price data for France (April 6–8, 2025) from the EPEX Spot auction site
- Cleaned and structured the data into a time series format (Datetime + Price)
- Calculated rolling 6-hour standard deviation to capture local volatility
- Used Z-score to detect hours with unusually high volatility (Z > 2)
- Built an ARIMA(2,1,1) model in Python to forecast the next 24 hours of prices
- Created a Power BI dashboard to visualize prices, volatility, and high-risk periods

---

## Tools

- **Python**: pandas, matplotlib, seaborn, statsmodels
- **Power BI**: For visualizing hourly price movements and risk markers
- **Data source**: [epexspot.com](https://www.epexspot.com/en/market-data)

---

## File Overview

```bash
.
├── electricity_volatility_analysis.ipynb   # main notebook
├── powerbi_ready.csv                       # cleaned data for visualization
├── powerbi_future_24.csv                   # 24-hour forecast output
├── screenshots/                            # Power BI graph preview
└── README.md
