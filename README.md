# Data Science Programming Project: UK Greenhouse Gas Emissions Analysis (2005–2022)

This repository contains a Jupyter Notebook analyzing UK greenhouse gas (GHG) emissions from 2005 to 2022. Using open government datasets, it demonstrates data wrangling with Pandas and NumPy, and data visualization using Matplotlib and Seaborn. The analysis ends with evidence-based insights and recommendations relevant to climate change mitigation.

## Project Highlights
Dataset Sourcing & Justification: Selected an open UK government dataset offering regional emissions by gas type and sector.

Data Cleaning & Preprocessing: Addressed missing values, dropped unnecessary columns, forward-filled time-series gaps, and capped outliers.

Exploratory Data Analysis (EDA): Identified trends by region, year, and sector; engineered per capita and per area emission metrics.

Visualization: Created insightful plots to explore emission trends and relationships between emissions, population, and geography.

Conclusions & Recommendations: Developed targeted, evidence-based policy suggestions using normalized data and rolling averages.

## Dataset Information
Source: data.gov.uk

Dataset Name: UK Greenhouse Gas Emissions: Local Authority and Regional

Link: View dataset

Last Updated: 27 June 2024

Why this dataset?
It includes emissions data by gas (CO₂, CH₄, N₂O), by region, and by sector. This granularity enabled emissions normalization (e.g., per capita, per km²) and robust comparisons across the UK.

## Notebook Overview (Assignment 2.ipynb)
### 1. Data Preparation
Imported data using Pandas; inspected structure and completeness.

Cleaned nulls and dropped non-essential columns.

Removed invalid (negative) emission records (~20,000 rows).

Applied 99th-percentile capping for outlier control.

### 2. Data Analysis & Visualization
Correlation Matrix: Weak but positive correlations among emissions, population, and area.

Trend Analysis: CO₂ shows a consistent decline, especially after 2008.

Rolling Averages: Smoothed short-term fluctuations using 3-year rolling mean.

Regional Breakdown: South East, North West, and Scotland are highest emitters.

Sectoral Analysis: Transport and Domestic are the leading emission sources.

Feature Engineering:

Per Capita Emissions – Scotland and Northern Ireland rank highest.

Emissions per Area – London has the highest emissions density.

### 3. Conclusions & Policy Recommendations
Urban Regions (e.g., London): Prioritize efficient transport, green infrastructure, and energy use reductions.

Rural Areas (e.g., Scotland, Northern Ireland): Support clean agriculture, renewables, and low-emission tech.

National Strategy: Use localized insights and rolling averages to inform sustainable, long-term decarbonization policies.

## Tools & Techniques
Data Tools: Pandas, NumPy

Visualization: Matplotlib, Seaborn

Techniques: Descriptive stats, outlier treatment, normalization, time series smoothing, group aggregations

## Challenges Addressed
Data Gaps: Forward-filled temporal data to preserve time continuity.

Outliers: Controlled skewed values using percentile capping.

Negative Values: Removed invalid data to ensure statistical integrity.

Complex Relationships: Engineered new features (per capita, per km²) to improve interpretability.
