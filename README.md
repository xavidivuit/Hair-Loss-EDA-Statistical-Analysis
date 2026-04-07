# Hair Loss EDA & Statistical Analysis

Exploratory data analysis of hair loss predictors in R, using a dataset of 999 individuals with clinical and lifestyle variables.

## Overview

This project explores the relationship between hair loss and a range of factors including stress levels, nutritional deficiencies, smoking, age, BMI, and medical conditions. The analysis is implemented as a fully reproducible R Markdown document.

## Workflow

### 1. Data Import & Management
- Load the dataset from `Predict Hair Fall.csv`
- Replace `"No Data"` entries with `NA`
- Summarise variable types, sample sizes and null value counts

### 2. Exploratory Analysis
- Proportion of stress levels grouped by nutritional deficiency
- Relationship between stress and hair loss (bar chart)
- Hair loss counts by nutritional deficiency type
- Filtered subsets: smokers below mean age with hair loss, grouped by stress level
- Youngest individuals with hair loss, high stress, smoking and medical treatment — nutritional deficiency profile

### 3. Visualizations
- Bar charts, boxplots, heatmaps, and histograms using `ggplot2` and base R
- Heat map of medical conditions by hair loss status
- Age distribution with empirical and theoretical normal density curves

### 4. Normality Assessment
- Shapiro-Wilk test on the age distribution of people with hair loss
- Q-Q plot for visual normality inspection

## Input File

| File | Description |
|---|---|
| `Predict Hair Fall.csv` | Dataset with 999 individuals and 13 variables including age, stress, smoking, nutritional deficiencies, medical conditions and hair loss status |

## Key Packages

| Package | Purpose |
|---|---|
| `readr` | CSV file import |
| `knitr` | Formatted tables in R Markdown |
| `ggplot2` | Data visualization |
| `dplyr` | Data manipulation and grouped summaries |

## How to Run

1. Clone this repository
2. Place `Predict Hair Fall.csv` in the project root
3. Open `Hair-Loss-EDA-Statistical-Analysis.Rmd` in RStudio
4. Click **Knit** to generate the HTML report
