# Bootstrapping Analysis of Environmental and Economic Indicators

This project demonstrates the application of **bootstrap methods** to quantify statistical uncertainty and assess the significance of analyses on environmental and economic indicators, focusing on **CO2 emissions per GDP** across countries with different income levels.

## Key Steps

### 1. Defining Income Groups
- GDP per capita data was used to classify countries into **low**, **medium**, and **high-income groups**.  
- Bootstrap resampling (2,000 replicates) was applied to estimate 95% confidence intervals for median GDP.  
- Parametric bootstrap thresholds were selected to define income categories:
  - Low: < \$11,609  
  - Medium: \$11,609–\$20,969  
  - High: > \$20,969  

### 2. Comparing CO2 Emissions
- Median CO2 intensity (CO2 per GDP) was compared between low- and high-income countries.  
- Non-parametric bootstrap (2,000 resamples) was used to estimate variability and confidence intervals.  
- Findings:
  - Median difference CI includes zero → difference not statistically significant  
  - Median ratio suggests low-income countries are slightly more CO2-efficient relative to GDP  

### 3. Environmental Kuznets Curve (EKC) Regression
- Modeled log(CO2) vs. log(GDP per capita) with a quadratic term.  
- Bootstrap (2,000 replicates) provided confidence intervals for regression coefficients and turning point.  
- Results:
  - Negative quadratic term confirms an **inverted-U shape**  
  - Turning point ~ \$16,209 GDP per capita (95% CI: \$12,647–\$24,957), marking where CO2 intensity starts declining  

## Conclusion
- Bootstrap methods provided **robust, data-driven thresholds** for income classification.  
- Resampling quantified uncertainty in median comparisons and regression estimates.  
- The analysis highlights bootstrap as a **powerful tool for statistical inference** without strong parametric assumptions.  

Overall, this project illustrates how bootstrap techniques can strengthen interpretation and confidence in environmental and economic data analyses.
