# Estimating Heterogeneous Treatment Effects with ML Method - Readme

## Introduction

This repository contains R code and analysis for estimating heterogeneous treatment effects using machine learning methods. The project is authored by Yiğit Kavak at LMU. The primary objective of this project is to investigate the impact of a policy change on gender wage gap and unemployment rates between the years 2005 and 2010 in the US.

## Prerequisites

Before running the code, ensure that you have the following libraries installed:

- `data.table`: Efficient data manipulation
- `hdm`: High-Dimensional Metrics and Bootstrap for Lasso
- `ggplot2`: Data visualization

Also, be sure that LaTeX is downloaded in your computer if you want to knit the Rmd file into a PDF file.

## Data

The dataset, named "genderinequality.csv", contains information about individuals' employment, wages, experience, tenure, and other variables for the years 2005 and 2010. The dataset is utilized to estimate the heterogeneous treatment effects on various economic variables.

## Analysis

### Treatment Effect on Gender Wage Gap

The main focus of this section is to examine the effect of the treatment on the gender wage gap, specifically the change in hourly wages between 2005 and 2010. Only individuals employed in both years are analyzed. A machine learning approach is employed to investigate the treatment effect heterogeneity. The analysis involves the following steps:

1. Data preprocessing: Filtering and merging data for the years 2005 and 2010.
2. Calculating variables: Computing relevant variables such as `change_hourly_wage`, `change_wage`, `change_exper`, `change_tenure`, and `change_emp`.
3. Constructing the model: Building a machine learning model to estimate heterogeneous treatment effects on the change in hourly wage while considering various covariates.
4. Coefficient summary: Summarizing the coefficients and their significance.

### Visualization

A visualization is generated to illustrate significant treatment effects by covariate. The covariates' treatment effects, along with their confidence intervals, are plotted to provide a clear understanding of the results.

### Treatment Effect on Change in Unemployment

Similar to the previous section, a machine learning approach is used to examine the treatment effect heterogeneity on the change in employment status (change in employment, layoff, or new employment) between 2005 and 2010. The analysis involves the following steps:

1. Data preprocessing: No special preprocessing is required for this section.
2. Constructing the model: Building a machine learning model to estimate heterogeneous treatment effects on the change in employment status while considering various covariates.
3. Coefficient summary: Summarizing the coefficients and their significance.

### Comments on Expected Impacts

In this section, the results are interpreted, focusing on the heterogeneity of treatment effects. The commentary delves into how different factors contribute to the variability in treatment effects across individuals.

### Implications for Germany

The discussion in this section emphasizes potential challenges in applying the same policy in Germany while accounting for the estimated heterogeneous treatment effects. Factors such as the different labor market structure, union influence, and economic context need to be considered before directly applying the US policy to Germany.

## Conclusion

This repository contains R code and analysis files that estimate heterogeneous treatment effects using machine learning methods. The analysis includes data preprocessing, model construction, coefficient summary, visualization, and interpretation of results. The insights gained from this analysis provide a valuable perspective on the heterogeneous impact of the policy in the US context and its potential implications for Germany.

Please contact Yiğit Kavak from fyigitkavak@icloud.com for further questions.