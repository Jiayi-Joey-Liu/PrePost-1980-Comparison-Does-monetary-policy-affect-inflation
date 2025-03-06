README: Empirical Economic Analysis - Final Project

Project Overview

This project analyzes the impact of the 1980 monetary policy shock on different industries using econometric techniques such as Regression Discontinuity (RD) and Two-Stage Least Squares (2SLS). Robustness checks are conducted using alternative instrumental variables and different time windows.

Folder Structure

The project is organized into the following directories:

data/ : Contains all the datasets used in the analysis.

programs/ : Contains MATLAB scripts for data processing, regression analysis, and robustness checks.

Figures/ : Contains visual outputs generated from the analysis.

Data Sources

The data/ folder includes the following datasets:

bbe.xls: Contains a wide range of macroeconomic time series, similar to the dataset of Bernanke, Boivin, and Eliasz (2005).

PCE_deflator.xls: Contains disaggregated PCE deflators (source: BEA).

PCE_quantities.xls: Contains disaggregated PCE quantity indices (source: BEA).

PPI.xls: Contains disaggregated producer price indices (source: BLS).

data_lists.xls: Indicates the descriptions and code names of series used. It also includes a sheet indicating which of the disaggregated PCE series have been included in the dataset.

data76.mat: MATLAB dataset containing transformed and processed data used in the econometric analysis.

weights.mat: MATLAB dataset containing 140 weights for calculating the weighted PCE.

Code Files

The programs/ folder includes the following key MATLAB scripts:

Team42_Project.m: The main script that runs the entire analysis, including data preprocessing, RD estimation, 2SLS estimation, and robustness checks.

2SLS_Robust_IVs.m: Implements robustness checks using different instrumental variables.

causal_analysis.m: Additional causal inference tests.

summary_stats.m: Computes and exports summary statistics for key variables.

3SLS_results.m: Implements Three-Stage Least Squares (3SLS) regression as an additional robustness check.

2SLS_results.m: Stores computed 2SLS regression results for different IV specifications.

B_industry_data.m: Processes industry-level data for analysis.

IRF_PCE_to_PPI_Shock_Fixed.m: Implements impulse response function analysis.

Industry_Group_Distribution.m: Groups industries for comparative analysis.

Output Files

The Figures/ folder contains graphical outputs and text-based results from the analysis:

PNG Files:

2SLS_Industry_Effects.png: Bar chart comparing 2SLS estimated effects for different industries.

2SLS_Comparison_IVs.png: Side-by-side comparison of 2SLS results using different instrumental variables.

RD_Bandwidth_12.png: Sensitivity tests for RD estimation using a bandwidth of 12.

RD_Bandwidth_24.png: Sensitivity tests for RD estimation using a bandwidth of 24.

RD_Bandwidth_36.png: Sensitivity tests for RD estimation using a bandwidth of 36.

RD_PCE_PPI.png: Regression Discontinuity analysis of PCE on PPI shocks.

IRF_PCE_to_PPI_Shock.png: Impulse response function analysis.

Variance_Decomposition.png: Displays variance decomposition results.

time_series_plot.png: Time series visualization of key variables.

seasonal_decomposition_fixed.png: Seasonal decomposition of key economic indicators.

RD_P1TDGG_B_Durable_goods.png: RD results for Durable Goods (P1).

RD_P1TNDG_B_Nondurable_goods.png: RD results for Nondurable Goods (P1).

RD_P1TSSG_B_Services.png: RD results for Services (P1).

RD_Q1TDG_B_Durable_goods.png: RD results for Durable Goods (Q1).

RD_Q1TND_B_Nondurable_goods.png: RD results for Nondurable Goods (Q1).

RD_Q1TSS_B_Services.png: RD results for Services (Q1).

B_Industry_TimeSeries.png: Time series plot of industry-level data.

Text Files:

2SLS_Results.txt: Summary of 2SLS regression estimates.

2SLS_Results_Consumer_Expectations.txt: 2SLS results using Consumer Expectations as IV.

2SLS_Results_FFR.txt: 2SLS results using Federal Funds Rate as IV.

2SLS_Results_M2.txt: 2SLS results using M2 money supply as IV.

Robustness_Tests_Results.txt: Summary of robustness checks.

regression_results.txt: Regression coefficients and model fit statistics.

Contact Information

For any questions regarding the project, please contact:

Jiayi (Joey) Liu

Yujin (Kim) Zhang

Hongyi (Clark) Zhong

Syed Irtiza Medhi

Demir Degirmenci