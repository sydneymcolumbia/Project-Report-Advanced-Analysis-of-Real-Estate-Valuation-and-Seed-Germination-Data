# Project-Report-Advanced-Analysis-of-Real-Estate-Valuation-and-Seed-Germination-Data
Project Report: Advanced Analysis of Real Estate Valuation and Seed Germination Data

Part I: Real Estate Valuation Analysis

Overview
The project commenced with an in-depth analysis of the 'real-estate-valuation-data-set.csv' from the UCI Machine Learning Repository. The dataset provided information on properties in New Taipei City, Taiwan, including the age of houses, distance to the nearest Mass Rapid Transit (MRT) station, number of convenience stores nearby, and unit price of houses.

Objectives & Methods
The analysis involved several steps:

Refined Multiple Linear Regression: The data was loaded in R. Based on observations from previous homework, a multiple linear regression was fitted with unit_price regressed on convenience_stores and the logarithm of distance.
Diagnostic Plot Analysis (Convenience Stores): Standardized residuals of the model were plotted against convenience_stores to identify potential model issues.
Diagnostic Plot Analysis (Logarithm of Distance): Similar diagnostic plots were created for the logarithm of distance.
Residuals vs. Fitted Values Plot: A plot of standardized residuals against fitted values of unit_price was generated to assess model adequacy.
Quantile-Quantile Plot of Residuals: This plot was created to examine the normality of residuals.
Box-Cox Transformation: The Box-Cox method was applied to find the optimal power λ for unit_price with the given predictors.
Regression with Transformed Response Variable: A multiple linear regression model was fitted with the transformed response variable unit_priceλ.
Diagnostic Plot Re-Evaluation: Diagnostic plots were recreated for the new model to assess improvements post Box-Cox transformation.
Influence Analysis: The influence.measures function in R was used to compute DFBETAs for the predictors, identifying influential observations.



Part II: Seed Germination Analysis

Overview
The project then shifted to analyzing the 'germ' dataset from the GLMsData library, which contained data on seed germination experiments with two types of extracts: beans and cucumbers.

Objectives & Methods
This section involved:

Logistic Regression Model: A logistic regression model was fitted for the proportion of germinated seeds (Germ / Total) onto the predictors Extract and Seeds.
Model Summary Analysis: The model summary was analyzed to answer specific questions regarding the baseline category of categorical predictors, odds of germination for different combinations of Extract and Seeds, and comparisons of odds of germination across different extract and seed types.
Deliverables

The project concluded with a detailed report encompassing findings from both parts. For the real estate data, the report not only provided a comprehensive statistical analysis but also offered insights into model diagnostics and improvements. The seed germination analysis provided a nuanced understanding of factors influencing germination rates in different conditions. The project demonstrated a sophisticated approach to data analysis, employing a variety of statistical techniques and interpretations to draw meaningful conclusions from diverse datasets.
