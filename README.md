# Wind Power and Emission Factor Analysis

## Description
This project combines data from two different APIs to analyze the relationship between wind power production and emission factors over time. The analysis was done using data from the Fingrid API. The emission factor data represents the carbon dioxide (CO₂) emission per kilowatt-hour (kWh) of electricity generated, while the wind power data represents the amount of electricity produced by wind turbines.

## Data Sources
- **Wind Power Data**: Fingrid API, dataset ID: 181
- **Emission Factor Data**: Fingrid API, dataset ID: 266

## Key Observations
1. **Flat Wind Power Production**: When wind power production remains relatively constant (flat), the emission factor also remains flat. This suggests that electricity generation from other sources (such as fossil fuels) is being used to meet the demand when wind power production is low.
  
2. **High Wind Power Production**: When wind power production spikes, the emission factor tends to drop. This indicates that higher wind power production is replacing electricity generation from fossil fuel sources, leading to a reduction in CO₂ emissions.

3. **Strong Negative Correlation**: The correlation between wind power production and the emission factor is **-0.92**, indicating a very strong negative relationship. As wind power production increases, the emission factor significantly decreases, suggesting that higher wind power production is effectively reducing CO₂ emissions by replacing fossil fuel-based generation.

## Requirements
- Python 3.10 or later
- `requests` library for API data fetching
- `pandas` library for data processing and analysis
- `matplotlib` library for data visualization

## Installation
To install the required libraries, run:
```bash
pip install requests pandas matplotlib

## AI Use
AI was used to write the documentation