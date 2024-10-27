# Neonicotinoid Concentration LC-MS Data Analysis in Freshwater Bodies (2024)

## Project Overview

This project conducts a comprehensive analysis of neonicotinoid concentrations in freshwater bodies across various sites in the UK. Utilizing data from the Environment Agency's LC-MS non-target monitoring database, the project employs Monte Carlo simulations, spatial mapping, and statistical analysis to assess neonicotinoid exceedance levels relative to industry-standard Environmental Quality Standards (EQS). The analysis aligns with regulatory frameworks, including the EU Water Framework Directive and ISO standards for environmental risk assessment.

## Key Objectives

- **Assess Neonicotinoid Concentrations:** Analyze levels of neonicotinoids such as Imidacloprid, Clothianidin, Acetamiprid, Thiamethoxam, and Thiacloprid across multiple UK sites.
- **Predict Future Contaminant Levels:** Use Monte Carlo simulations to forecast future concentrations and evaluate potential ecological risks.
- **Map High-Risk Areas:** Conduct spatial mapping to identify geographical hotspots where neonicotinoid levels exceed EQS thresholds.
- **Align with Regulatory Standards:** Ensure analysis aligns with the EU Water Framework Directive and ISO 31010 guidelines for risk assessment.

## Data Sources

Data for this project is derived from The Rivers Trust and Wildlife and Countryside Link's analysis of Environment Agency monitoring data:
- **Dataset:** Includes summaries from files such as `5_neonics_summary_web_sept_2023.xlsx` and detailed analysis in `Neonic_research_individual_chemicals_summary_web_sept_2023.docx`.
- **Variables Included:**
  - `Site ID`: Unique identifier for each monitoring site.
  - `Compound Name`: Name of the neonicotinoid (e.g., Imidacloprid).
  - `Mean Concentration (ug/L)`: Average concentration levels.
  - `Latitude` and `Longitude`: Geographic coordinates for spatial mapping.
  - `Exceedance of AA-EQS`: Assessment of whether concentrations exceed the Acceptable Annual EQS thresholds.

## Methods

### 1. Data Preprocessing

- Loaded and cleaned data using `pandas`, handling missing values and ensuring consistent column formatting.
- Filtered data for key neonicotinoids and calculated exceedance levels relative to AA-EQS standards.

### 2. Statistical Analysis

- **Distribution Analysis:** Created boxplots to visualize neonicotinoid concentration distributions across sites.
- **Correlation Analysis:** Generated a correlation matrix to examine relationships among different neonicotinoids.
- **Validation Metrics:** Used metrics like Mean Squared Error (MSE) and Root Mean Squared Error (RMSE) to assess model predictions.

### 3. Predictive Modeling with Monte Carlo Simulation

- **Simulation Method:** Conducted Monte Carlo simulations to forecast future concentrations of Imidacloprid over a 10-year horizon.
- **Alignment with ISO 31010:** Simulation approach aligns with ISO 31010 for risk assessment in uncertain environmental conditions.
- **Interpretation of Results:** Simulations suggest potential increases in Imidacloprid levels over time, with exceedances in several regions.

### 4. Spatial Mapping

- **Geographic Analysis:** Utilized `folium` to create interactive maps identifying hotspots of neonicotinoid exceedance.
- **Risk Visualization:** Visualized pollutant concentration levels relative to AA-EQS benchmarks to highlight areas of concern.
- **Regulatory Application:** Findings support the Environment Agency in prioritizing locations for mitigation and regulatory action.

## Key Findings

- **Identified Hotspots:** Key sites like `RSN RUNNING WATERS RUXOX BRIDGE` and `OLD FORGE FARM SOMERHILL STREAM` exhibited Imidacloprid concentrations significantly above AA-EQS thresholds.
- **Predictive Accuracy:** The Monte Carlo simulation for Imidacloprid indicated an RMSE of `0.071`, suggesting high accuracy in predictions.
- **Correlation Insights:** The correlation matrix showed moderate negative correlations between Imidacloprid and Thiacloprid, hinting at potential competitive environmental interactions.

## Alignment with Industry Standards

- **Regulatory Compliance:** Analysis is consistent with the EU Water Framework Directive for assessing priority substances and exceedance metrics.
- **Risk Assessment Standards:** Monte Carlo simulations align with ISO 31010 standards for risk assessment under uncertainty.
- **Geospatial Data Management:** Data handling and mapping align with ISO 19115 standards for geographic information, ensuring precise location-based risk assessment.

## Recommendations

1. **Targeted Regulation:** Sites with Imidacloprid concentrations above x3 EQS thresholds should be prioritized for intervention.
2. **Long-term Monitoring:** Continued monitoring is essential in identified hotspots to track changes in concentration levels and inform regulatory adjustments.
3. **Mitigation Strategies:** Adopt precision agriculture techniques to reduce neonicotinoid runoff in high-risk regions.

## Next Steps

- **Broaden Chemical Scope:** Future studies could include additional pesticides and examine potential interactions between different chemical classes.
- **Incorporate Real-Time Data:** Integrate real-time sensor data to improve prediction accuracy and risk assessment capabilities.
- **Regulatory Collaboration:** Engage with agencies like the Environment Agency to apply findings in environmental policy frameworks.

## Visualizations and Files

### 1. [Top 10 Sites by EQS Exceedance](https://github.com/auwalmusa/pesticide-data-analysis/blob/main/Bar.png)
![Top 10 Sites by EQS Exceedance](https://github.com/auwalmusa/pesticide-data-analysis/blob/main/Bar.png)

### 2. [Distribution of Neonicotinoid Concentrations](https://github.com/auwalmusa/pesticide-data-analysis/blob/main/boxplot.png)
![Boxplot of Neonicotinoid Concentrations](https://github.com/auwalmusa/pesticide-data-analysis/blob/main/boxplot.png)

### 3. [Correlation Matrix](https://github.com/auwalmusa/pesticide-data-analysis/blob/main/correlation.png)
![Correlation Matrix](https://github.com/auwalmusa/pesticide-data-analysis/blob/main/correlation.png)

### 4. [Neonicotinoid Sites Map](https://github.com/auwalmusa/pesticide-data-analysis/blob/main/neonicotinoid_sites_map.html)
Interactive map showing sites with exceedances.
