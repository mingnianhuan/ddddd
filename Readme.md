# China Oil Price Analysis: A Comparative Study of National Price Adjustments and Regional Prices in Guangxi

## 1. Problems and Users
This project analyzes the impact of China’s refined oil price regulation mechanism on the actual retail prices in Guangxi. It helps consumers understand the fluctuation rules of oil prices and provides quantitative references for energy researchers to explore regional price differences.

## 2. Data
*   **Source**: Akshare financial data interface library
  - Historical price adjustment data: `ak.energy_oil_hist()`
  - Regional detailed data: `ak.energy_oil_detail(date=YYYYMMDD)`
*   **Time Range**: 2024–2025 (the latest available data)
*   **Key Fields**: Price adjustment date, national adjusted price (yuan/ton), 92# gasoline price in Guangxi (yuan/liter)

## 3. Methods & Tech Stack
*   **Main Process**: Data collection → Data cleaning and conversion → Price comparative analysis → Price difference calculation → Month-on-month growth analysis → Visual presentation
*   **Tech Stack**:
  - Data processing: `pandas`
  - Data acquisition: `akshare`
  - Visualization: `matplotlib`

## 4. Core Findings
*   **Price Difference Rule**: There is a noticeable price gap between retail prices in Guangxi and national adjusted prices, reflecting regional costs such as logistics and operation expenses.
*   **Fluctuation Follow-up Feature**: Price changes in Guangxi are highly correlated with national price adjustments, with a delayed response of 1–2 days.
*   **Cost Structure Analysis**: Calculated by the minimum price difference, the fixed logistics and operating cost in Guangxi is about 768.720 yuan/liter.

## 5. How to Run
pip install -r requirements.txt

## 6. Data Analysis Dimensions
1. **Price Trend Comparison**: National adjusted price vs. actual retail price in Guangxi
2. **Month-on-Month Growth Rate**: Change rate between adjacent price adjustment dates
3. **Price Difference Analysis**: Quantification of regional costs
4. **Market Follow-up**: Response degree of regional prices to national policy adjustments
5. **Cost Structure Inversion**: Estimate fixed and variable costs based on price difference data

## 7. Key Outputs
*   **Chart 1**: Trend comparison of national oil price adjustment and Guangxi price (dual Y-axis)
*   **Chart 2**: Month-on-month growth rate comparison between nationwide and Guangxi
*   **Console Output**:
  - Analysis period and total data volume
  - Price statistics (mean value, value range)
  - Price difference analysis (average, maximum, minimum gap)
  - Month-on-month growth rate statistics
  - In-depth analysis (fixed cost estimation, market efficiency coefficient)

## 8. Limitations & Optimization
### Current Limitations
*   **Cost Segmentation**: Detailed data of logistics, taxation and operating costs cannot be obtained.

### Future Optimization Directions
1. **Multi-region Comparison**: Expand the research scope to 31 provinces, municipalities and autonomous regions across the country
2. **Influencing Factor Analysis**: Add international crude oil price, exchange rate and seasonal factors
3. **Prediction Model**: Establish oil price forecasting models based on time series analysis
4. **Interactive Visualization**: Build interactive dashboards with Plotly / Dash

## 9. AI Usage Statement
AI assistance was adopted in the following parts of this project:
*   **Visualization Optimization**: Layout and color matching suggestions for dual Y-axis charts

**Important Notice**: All data analysis logic, professional insights and research conclusions are completed manually. AI only serves as an auxiliary tool.