# Firearm Sales and Gun Deaths in Florida

## Overview

This project explores the relationship between firearm sales (as measured by background checks) and gun deaths in the state of Florida. Using publicly available datasets from Kaggle, the analysis aims to determine if there is a correlation between the number of background checks for firearm purchases and the number of firearm-related deaths over time.

## Research Questions

1. Have background checks increased in Florida over time?
2. Who is purchasing the most firearms in Florida (demographics)?
3. Is there monetary data available for purchases of firearms?
4. What has been the trend in gun deaths in Florida over time?
5. Is there a positive correlation between gun deaths and firearm purchases in Florida?

## Data Sources

- **Background Checks:** FBI NICS background check data  
  [Kaggle Link](https://www.kaggle.com/datasets/saurabhshahane/fbi-criminal-background)
- **Population Data:** U.S. Census ACS 2017  
  [Kaggle Link](https://www.kaggle.com/datasets/peretzcohen/2019-census-us-population-data-by-state)
- **Gun Deaths:** U.S. gun deaths by county (1999–2019)  
  [Kaggle Link](https://www.kaggle.com/datasets/ahmedeltom/us-gun-deaths-by-county-19992019)

## Methodology

The analysis was conducted using R, employing the following steps:

- **Data Cleaning & Filtering:** Each dataset was filtered to include only records from Florida. Due to limitations in the population dataset (available only for 2017), some comparisons are year-specific.
- **Exploratory Data Analysis (EDA):** Scatter plots, histograms, and summary statistics were used to explore background check trends and death counts.
- **Statistical Modeling:** Simple linear regression models were used to assess the relationship between background checks and time, as well as gun deaths and time.

## Key Findings

- There is a **positive linear trend** in both background checks and gun deaths over time in Florida.
- Linear regression analysis yielded statistically significant results, suggesting a reliable correlation between year and firearm-related activity.
- Limitations include the inability to merge datasets cleanly and a lack of multivariate regression modeling incorporating population and demographic data.

## Tools and Packages Used

- `dplyr` – data manipulation  
- `ggplot2` – data visualization  
- `coefplot` – regression coefficient visualization  
- `readr` – data import

## Limitations & Future Work

- Expand the analysis across multiple years and states.
- Include demographic and population-adjusted metrics.
- Incorporate multiple regression and classification models to improve insights.

## File Descriptions

- `analysis_background_checks.R` – R script for data cleaning, EDA, and modeling  
- `Analysis of Background Checks.pdf` – Full project report including visualizations, methodology, and conclusions

---

Ruben Brionez Jr  
March 2024
