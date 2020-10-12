# CS1-Practice

## Analyzing Health Nutrition & Population Statistics Compiled by the World Bank
### Dustin Eubanks

This analysis was performed using publicly available data on Health, Nutrition & Population statistics from the World Bank.  The dataset is publicly available on the World Bank website [link](https://datacatalog.worldbank.org/dataset/health-nutrition-and-population-statistics) but was obtained in raw form from Kaggle [link](https://www.kaggle.com/theworldbank/health-nutrition-and-population-statistics) for the contents of this report.  An excerpt explaining the Context & Content of the dataset, from Kaggle:

>
**Context**
HealthStats provides key health, nutrition and population statistics gathered from a variety of international sources. Themes include population dynamics, nutrition, reproductive health, health financing, medical resources and usage, immunization, infectious diseases, HIV/AIDS, DALY, population projections and lending. HealthStats also includes health, nutrition and population statistics by wealth quintiles.
>
**Content**
This dataset includes 345 indicators, such as immunization rates, malnutrition prevalence, and vitamin A supplementation rates across 263 countries around the world. Data was collected on a yearly basis from 1960-2016.


There are a number of other analysis reports on this dataset available on Kaggle [here](https://www.kaggle.com/theworldbank/health-nutrition-and-population-statistics/notebooks).  Inspiration for this report was often obtained from those examples, and is credited below.


## Summary

The analysis approach for this report was exploratory with no hypotheses in mind prior to examining the data.  The data was loaded in raw form using Python/Pandas, reviewed, and then plotted with Matplotlib to visualize and identify any potentially interesting trends or comparisons.

An initial review of the dataset revealed the following attributes:

* Shape: 89,010 rows, 61 columns (5,429,610 cells)
* Completeness: 2,597,528 NaN values (roughly 47% of total cells)
* Contents:
    - 345 Unique Indicators (Health/Population)
    - 258 Unique Groups (Regional, Geographic or Demographic)

Quite a massive data set, but missing a lot of information (empty cells) as well.  Using Pandas we slice the data down to get a sense of the features available:

### Indicators
The 345 unique indicators were arranged into a subset of the data:

![Indicators](https://github.com/eubanksd55/CS1-Practice/blob/main/indicators.png?raw=true)

### Groups
The 258 unique groups were arranged into a subset of the data:

![Groups](https://github.com/eubanksd55/CS1-Practice/blob/main/groups.png?raw=true)

