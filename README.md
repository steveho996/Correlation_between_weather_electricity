# Report website for correlation between weather and electricity price

---

This case study demonstrates how I built an end-to-end report website with real Finland electricity data using Python and Power Query, following a clear ETL flow, and loading the entire project to GitHub via VS Code. This interactive data visualization dashboard provides insights into Finnish electricity consumption, pricing trends, and temperature variations over a selected period. By analyzing real-world electricity usage data, the dashboard helps users understand how energy consumption fluctuates and how pricing impacts overall electricity costs.


## ETL Flow

### 1. Extract
- Source: CSV files exported from logistics operations database
- Files loaded into **Power Query** to inspect data structure, types, and quality

### 2. Transform
- Data cleaned and standardized using **Power Query**:

### 3. Load
- Cleaned CSV files loaded into **PostgreSQL**
- Build correlation visualisation between weather and electricity price
- Analyst the correlation
- Publish on website via streamline

## Report 

### Correlation Heatmap

This table presents key descriptive statistics for three variables:A positive correlation (closer to +1) means that as one variable increases, the other tends toincrease as well, while a negative correlation (closer to -1) indicates an inverse relationship. Acorrelation near 0 suggests little to no relationship.
1/ Temperature has a weak positive correlation (0.15) with electricity prices, meaning that astemperature increases, prices tend to rise slightly. However, the relationship is weak,suggesting that other factors (such as demand, energy production, or external economicconditions) play a more significant role.
2/ Wind speed has almost no correlation (-0.02) with electricity prices, implying thatfluctuations in wind speed alone do not have a direct impact on pricing. This may be due toFinland’s energy mix, where wind power is not the dominant pricing factor.
3/ Temperature and wind speed have a slight negative correlation (-0.077), meaning that highertemperatures are slightly associated with lower wind speeds, though the relationship is weak.

<img width="588" height="469" alt="Capture" src="https://github.com/user-attachments/assets/f3ec1094-12d8-4d1a-a13a-cf985855b37b" />

### Actual Prices and Predicted Prices

<img width="709" height="564" alt="Capture 2" src="https://github.com/user-attachments/assets/636a66b2-8dd5-4a3c-8373-195fd04a284f" />

### Impact of Temperature on Price

Based on the provided visualization, a scatter plot, the analysis reveals a significantrelationship between temperature and electricity prices.The visualization demonstrates an inverse correlation between temperature speed andelectricity prices:
1/ Higher wind speeds lead to lower and more stable electricity prices.
2/ Low wind speeds are linked to greater price volatility and higher costs.

<img width="721" height="540" alt="Capture 3" src="https://github.com/user-attachments/assets/6742d0c0-ac84-44f4-b402-ff9e271764cc" />

### Impact of Wind speed on Price

Based on the provided visualization, a scatter plot, the analysis reveals a significantrelationship between wind speed and electricity prices.Higher wind speeds are linked to lower and more stable electricity prices, likely reflecting thecost benefits of increased wind energy production.Conversely, low wind speeds result in higher and more volatile prices, emphasizing thechallenges of limited renewable energy availability during calm periods.

<img width="705" height="532" alt="Capture 4" src="https://github.com/user-attachments/assets/e22b17a8-05b8-445f-80c2-afd9f4fd054f" />

