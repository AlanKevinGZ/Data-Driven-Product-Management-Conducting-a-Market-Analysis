# Data-Driven-Product-Management-Conducting-a-Market-Analysis

## Overview

This project analyzes worldwide and country-level Google search trends related to workout habits.  
The objective is to understand how fitness behavior changed during the COVID-19 pandemic and determine current preferences to support data-driven decisions.

The analysis focuses on time series reasoning, filtering, aggregation, and visualization using Python and pandas.

---

## Objectives

- Identify the most popular workout type during the COVID pandemic
- Determine the most popular workout type currently
- Compare the Philippines and Malaysia to decide where to expand a home workout offering

---

## Dataset Description

### three_keywords.csv
Monthly worldwide search interest for:
- home_workout_worldwide
- gym_workout_worldwide
- home_gym_worldwide

### three_keywords_geo.csv
Country-level search interest for the same workout categories.

---

## Methodology

### Pandemic Analysis (Time Series)

- Filtered dates between 2020 and 2023
- Compared keyword peaks during the pandemic
- Used maximum value detection to find the most popular trend

Key idea:
Historical peak ≠ current popularity

---

### Current Trend Detection

- Sorted data by date descending
- Selected only the most recent month
- Compared values within that single row

Key idea:
For "current" values, use the latest observation, not the global maximum

---

### Country Comparison

- Filtered only Philippines and Malaysia
- Compared home workout interest directly
- Selected the country with the highest value

Key idea:
Categorical comparisons require direct value comparison

---

## Visualization

Different charts were used depending on the structure of the data:

### Line Chart
Used for time series data
- Shows trends and behavior changes over time
- Helps detect spikes during COVID and current dominance

### Bar Chart
Used for country comparison
- Best for discrete categories
- Makes magnitude differences easier to interpret

---

## Skills Demonstrated

- Data cleaning with pandas
- Boolean filtering
- Time series analysis
- Index-based selection (idxmax)
- Sorting and row extraction
- Data visualization with matplotlib
- Analytical thinking for correct metric selection

---

## Tools

- Python
- pandas
- matplotlib

---

## Key Learnings

- Use line plots for time-dependent data
- Use bar charts for categorical comparisons
- Always match the analysis method to the problem context
- Correct interpretation of time is critical in trend analysis
