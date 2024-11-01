---

# Ad Campaign Performance Analysis

## Project Overview

This project analyzes the performance of two ad campaigns conducted by a marketing agency across two platforms: Facebook and AdWords. The goal is to determine which platform yields better results in terms of clicks, conversions, and overall cost-effectiveness. The findings will enable us to make data-driven recommendations for optimizing advertising strategy and maximizing return on investment (ROI) for future campaigns.

## Business Problem

Advertising budgets are often constrained, and each campaign's effectiveness significantly impacts overall ROI. To ensure resources are allocated optimally, it is crucial to identify which ad platform performs better. This project focuses on addressing the following questions:

1. Which ad platform—Facebook or AdWords—delivers higher conversions and clicks?
2. Which platform is more cost-effective in achieving conversions?

## Dataset Description

The dataset covers daily performance metrics of Facebook and AdWords ad campaigns over the year 2019. Each row corresponds to a day's data, totaling 365 records, and includes the following key features:

- Date: Date of the ad performance metric (daily from January 1, 2019, to December 31, 2019)
- Ad Views: Number of times the ad was viewed
- Ad Clicks: Number of clicks on the ad
- Ad Conversions: Number of conversions generated from the ad
- Cost per Ad: Cost associated with running the ad campaign for that day
- Click-Through Rate (CTR): Ratio of clicks to views
- Conversion Rate: Ratio of conversions to clicks
- Cost per Click (CPC): Average cost incurred per click

## Methodology

The analysis is organized into the following steps to answer the business question methodically:

### 1. Exploratory Data Analysis (EDA)

   - Objective: Gain insights into the distribution, trends, and relationships between the features for both ad platforms.
   - Steps:
     - Load and inspect data, including summary statistics for each platform.
     - Visualize trends in ad views, clicks, and conversions over time.
     - Compare average CTR, conversion rate, and CPC between Facebook and AdWords.

### 2. Hypothesis Testing

   - Objective: Determine if the differences between Facebook and AdWords campaign metrics (clicks, conversions, cost-effectiveness) are statistically significant.
   - Hypothesis:
      - Null Hypothesis (H0): There is no significant difference between Facebook and AdWords in terms of conversions, clicks, or cost-effectiveness.
      - Alternative Hypothesis (H1): There is a significant difference between Facebook and AdWords in terms of these metrics.
   - Tests Conducted:
      - T-tests for comparing means of continuous variables (e.g., CPC, CTR, and conversion rates).
      - Chi-square test if applicable for categorical analysis of outcomes.

### 3. Regression Analysis

   - Objective: Assess the influence of different factors (e.g., ad views, CTR, CPC) on conversions and clicks, helping identify key drivers of ad performance.
   - Approach:
      - Linear Regression: For continuous outcomes like clicks and conversions to determine which variables significantly impact performance.
      - Assumptions Check: Validate model assumptions (linearity, normality, multicollinearity) to ensure reliable results.
      - Interpretation: Evaluate coefficients to understand the impact of each factor on ad success metrics.

### 4. Results Interpretation

   - A/B Test Outcomes: Summarize any significant findings from hypothesis testing to determine platform effectiveness.
   - Regression Findings: Highlight key predictors of ad success and provide insight into potential optimizations.

## Conclusion

This analysis provides clear, data-driven recommendations for ad platform selection and highlights actionable insights on the variables that drive higher conversions and cost-efficiency. The final report includes:

- Summary of findings for each analysis step
- Recommendations for ad budget allocation based on ad performance
- Suggestions for further analysis, such as segmentation or more granular breakdowns by audience demographics

## Requirements

- Python Libraries:
  - pandas and numpy for data manipulation
  - matplotlib and seaborn for data visualization
  - scipy and statsmodels for hypothesis testing and regression analysis

## How to Use the Project

1. Clone the repository and ensure the dataset is in the working directory.
2. Install required packages by running:
   ```bash
   pip install pandas numpy matplotlib seaborn scipy statsmodels
   ```
3. Run the notebook to view each step of the analysis, from data exploration to regression analysis and interpretation.

## Future Scope

This analysis can be expanded by incorporating audience demographic information or conducting time-series forecasting to predict future ad performance based on seasonality trends.

---
