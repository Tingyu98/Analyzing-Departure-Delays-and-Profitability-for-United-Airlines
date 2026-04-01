# Departure Delays and Profitability Analysis for United Airlines

## Key Highlights
- Analyzed United Airlines flight performance using the nycflights13 dataset  
- Identified key drivers of departure delays including time of day, seasonality, and weather conditions  
- Established statistical relationships between delays and profitability using hypothesis testing  
- Derived actionable insights for improving operational efficiency and flight profitability  

---

## Overview
This project analyzes departure delays and profitability for United Airlines using the nycflights13 dataset.

By combining exploratory data analysis, statistical testing, and data integration with weather data, the project identifies key factors affecting flight delays and evaluates how operational efficiency impacts profitability.

---

## Key Questions
- What factors contribute most to flight departure delays?  
- How do time of day and seasonality affect delays?  
- How do weather conditions impact operational performance?  
- How does punctuality influence airline profitability?  

---

## Methodology
- **Data**: nycflights13 dataset (filtered for United Airlines flights)  
- **Feature Engineering**:  
  - Created delay indicators (late, very_late)  
  - Computed net gain (departure delay - arrival delay)  
  - Calculated gain per hour for profitability analysis  
- **Data Integration**: Merged flight data with weather dataset  
- **EDA**:  
  - Time-based analysis (hour, month)  
  - Distribution and trend visualization  
- **Statistical Analysis**:  
  - t-tests to compare group differences (on-time vs delayed flights)  
  - Permutation tests for time-of-day and seasonal comparisons  
- **Visualization**: Built using R (ggplot2)  

---

## Results & Insights

### Delay Analysis
- Departure delays increase throughout the day, peaking in evening hours (~5 PM) :contentReference[oaicite:2]{index=2}  
- Summer months and December show higher delays due to increased travel demand :contentReference[oaicite:3]{index=3}  
- Weather factors significantly impact delays:  
  - Higher temperature (>60°F) correlates with increased delays  
  - Increased wind speed and precipitation lead to higher delays  
  - Low visibility (<2.5 miles) strongly associated with delays :contentReference[oaicite:4]{index=4}  

### Profitability Analysis
- Flights departing on time generate significantly higher net gain (p < 2.2e-16) :contentReference[oaicite:5]{index=5}  
- Shorter flights yield higher gain per hour compared to longer flights :contentReference[oaicite:6]{index=6}  
- Popular routes (e.g., SFO) show higher profitability than less frequent routes (e.g., IAH) :contentReference[oaicite:7]{index=7}  

---

## Impact
- Demonstrates how operational delays directly affect airline profitability  
- Provides data-driven insights for improving scheduling and route optimization  
- Supports decision-making in airline operations and resource allocation  

---

## Use Cases
- Airline operations teams optimizing schedules and reducing delays  
- Route planning and profitability analysis  
- Aviation analytics and performance monitoring  

---

## Tech Stack
- R (dplyr, ggplot2)  
- Statistical Analysis (t-test, permutation test)  
- Data integration and feature engineering  

---

## Future Work
- Incorporate predictive modeling for delay forecasting  
- Extend analysis to multiple airlines and airports  
- Build real-time dashboards for operational monitoring  
- Integrate additional external data sources (e.g., air traffic, holidays)  
