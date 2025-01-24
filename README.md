# Energy Consumption Optimization
 


## Project Overview

This project for Carerha training first program’s final designed to apply the knowledge acquired during this course.

It focuses on analyzing and optimizing energy consumption data from various cells, with the goal of identifying low-demand cells where energy usage can be reduced to save both energy and costs. Through a series of statistical analyses and data visualizations, the project aims to uncover trends, identify key factors affecting energy consumption, and propose actionable insights to minimize energy waste.

## Key Objectives

1. **Data Analysis**: Explore and clean the energy consumption and damand data to extract useful insights and understand patterns.
2. **Statistical Testing**: Validate assumptions about the relationship between region, time of day, and energy consumption using statistical hypothesis tests.
3. **Threshold Determination**: Propose a threshold to identify low-demand cells and calculate the potential energy savings in kilowatt-hours (KW) and financial savings in Egyptian Pounds (EGP).
4. **Cost Reduction**: Calculate how much energy and money could be saved by reducing the energy consumption of low-demand cells.

## Methodology

### 1. Data Cleaning & Preprocessing
- **Handling missing data**: All missing date intervals and invalid data points were addressed to ensure the dataset is complete and reliable.
- **Outlier detection & handling**: Outliers in energy consumption values were identified and managed using the IQR (Interquartile Range) method, with extreme values replaced by the median.

### 2. Exploratory Data Analysis (EDA)
- **Statistical analysis** was performed to uncover patterns in energy consumption across regions, times of day, and demand levels.
- **Visualizations**: Various plots were created to better understand the data distribution and trends.

### 3. Energy Optimization & Threshold Determination
- A threshold based on the 25th percentile (Q1) of energy consumption was identified to define low-demand cells.
- **Energy savings calculations** were made based on this threshold, showing potential savings of 5183.44 KW and 1049.48 EGP by reducing energy usage in low-demand cells.

## Main challenges identified and proposed solutions

- **Extreme Outliers**: The data contained extreme outliers in the energy column, skewing the mean and standard deviation, making it difficult to analyze trends or perform statistical tests effectively, So used the Interquartile Range (IQR) method to detect outliers. Replaced outliers with the median value.

- **Missing Records**: The data had missing records for some date intervals across various regions. This created gaps in data, which could lead to inaccurate analyses.  So had to Identify Missing Records, Used the median energy for the respective region to fill in the missing records.

- **Improved Granularity**: The DateTime column in energy consumption data was critical for analyzing energy usage trends over time, but it was not in correct usable format and could use more deeper levels of granularity. So had to standardize the format and created additional columns for deeper analysis.


