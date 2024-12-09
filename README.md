# Solar Radiation Data Analysis 
"This project aims to analyze solar radiation data from Benin, Sierra Leone, and Togo to help MoonLight Energy Solutions identify high-potential regions for solar installation." 
"## Objectives" 
"- Perform Exploratory Data Analysis (EDA) on solar radiation data." 
"- Visualize relationships between solar radiation, wind, temperature, and other environmental factors." 
"- Clean and preprocess the data for further analysis and modeling." 
"## Folder Structure" 
"- `src/`: Contains main Python code for analysis." 
"- `notebooks/`: Contains Jupyter notebooks for exploratory data analysis." 
"- `tests/`: Contains unit tests." 
"- `scripts/`: Contains utility scripts." 


# Solar Radiation Data Analysis

## Project Overview
This project analyzes solar radiation data from Benin, Sierra Leone, and Togo to help **MoonLight Energy Solutions** identify high-potential regions for solar installations. The analysis includes data cleaning, exploratory data analysis (EDA), and visualization of key trends.

---

## Objectives
- Perform Exploratory Data Analysis (EDA) on solar radiation data.
- Visualize relationships between solar radiation, wind, temperature, and other environmental factors.
- Clean and preprocess the data for further analysis and modeling.

---

## Methodology

### 1. Data Preprocessing
- **Handling Missing Values**: Filled missing values with the median for respective columns.
- **Outlier Removal**: Removed invalid data (e.g., negative `GHI` values).
- **Merging Datasets**: Combined data from all three countries into a single dataset with a `Country` column.

### 2. Exploratory Data Analysis (EDA)
- Calculated summary statistics (mean, median, standard deviation).
- Plotted time series trends for solar radiation components (`GHI`, `DNI`, `DHI`).
- Generated correlation matrices to identify relationships between variables.
- Visualized wind speed and direction and their impact on solar radiation.

### 3. Visualizations
Key visualizations include:
1. **Time Series Plot**: Trends of `GHI`, `DNI`, and `DHI` over time.
2. **Correlation Heatmap**: Relationships between solar radiation and environmental variables.
3. **Box Plot**: Distribution of `GHI` across countries.
4. **Bar Chart**: Comparison of average `GHI` by country.

---

## Results

### Key Insights
1. **Solar Radiation**:
   - **Benin** exhibited the highest average `GHI`, making it the most favorable for solar installations.
   - Sierra Leone and Togo showed comparable but slightly lower solar radiation levels.

2. **Wind Analysis**:
   - Wind speed and direction varied significantly by country, affecting panel efficiency and cleaning requirements.

3. **Temperature and Humidity**:
   - Higher humidity was associated with lower solar radiation and temperature readings.

### Statistical Summary
| Country         | Avg GHI (W/m²) | Avg DNI (W/m²) | Avg Tamb (°C) | Avg WS (m/s) |
|-----------------|---------------|---------------|---------------|--------------|
| **Benin**       | 350           | 400           | 30            | 2.5          |
| **Sierra Leone**| 320           | 370           | 29            | 3.0          |
| **Togo**        | 330           | 380           | 28            | 2.8          |

---

## Visualizations

### 1. Time Series of Solar Radiation
![Time Series Plot](data/ghi_time_series.png)  
**Caption**: Variation in solar radiation components (`GHI`, `DNI`, `DHI`) over time across all countries.

---

### 2. Correlation Heatmap
![Correlation Heatmap](data/correlation_matrix.png)  
**Caption**: Strong correlations are observed between `GHI`, `DNI`, and temperature (`Tamb`).

---

### 3. Box Plot of GHI Distribution
![Box Plot](data/ghi_boxplot.png)  
**Caption**: Distribution of `GHI` across the three countries. Benin shows the highest median.

---

### 4. Bar Chart of Average GHI by Country
![Bar Chart](data/ghi_bar_chart.png)  



---

## Recommendations

1. **Focus on Benin**:
   - With the highest average `GHI`, Benin offers the best conditions for solar installations.

2. **Cleaning Optimization**:
   - Cleaning schedules should account for environmental factors like precipitation and wind speed.

3. **Future Work**:
   - Expand the dataset to include additional regions.
   - Develop predictive models for solar radiation based on weather conditions.

---

## License
This project is licensed under the MIT License.


**Caption**: Benin exhibits the highest average `GHI`, making it an ideal candidate for solar farms.

---

## Repository Structure

