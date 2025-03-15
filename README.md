# Expedia-Price-Sensitivity-Analysis-using-R
##Expedia Price Sensitivity Analysis

## Project Background

The purpose of this project was to conduct an experiment to understand consumer sensitivity to price changes in hotel bookings. This project analyzes whether prior observational estimates (a 20% decrease in bookings per $100 increase in price) align with experimental results and examines if price sensitivity varies by destination and customer income levels.

## Problem Statement

Traditional observational methods estimated that a $100 price increase results in a 20% drop in booking likelihood. However, recent research suggests that experimental data provides better estimates. This study aims to:

Validate prior observational estimates.

Measure true consumer price sensitivity using experimental pricing changes.

Analyze how price sensitivity differs across destinations and customer income levels.

### Key Questions

How does price affect booking probability?

Was the previous observational estimate of price sensitivity accurate?

Do different regions and income groups exhibit varying price sensitivity?

## Data Overview

This analysis utilizes experimentally collected data for a subset of hotels in multiple US markets. Only logged-in customers (with available income estimates) were included to ensure complete income data.

<img width="573" alt="image" src="https://github.com/user-attachments/assets/313b437e-358e-4704-946a-074f8e2279c2" />

## Methodology

Descriptive Analysis: Summary statistics of key variables.

Price Sensitivity Estimation: Linear regression to estimate the impact of price on booking probability.

Regional & Income-Based Sensitivity: Interaction models evaluating price sensitivity by region and income group.

Model Evaluation: Comparison of experimental findings with prior observational estimates.

We use a linear probability model.

Expected outcome: A negative coefficient on PricePerNight, indicating that higher prices reduce bookings.

Additional models include region- and income-based interactions to assess heterogeneity.

## Key Findings & Insights

### 1. How does price impact booking probability?

The estimated coefficient for PricePerNight is -0.00075, indicating that a $100 price increase leads to a 7.5% drop in booking probability.

The experimental estimate suggests a smaller effect than the prior observational estimate (20%).

![image](https://github.com/user-attachments/assets/c878890e-ef01-4e26-b065-a996c8e41bd1)


### 2. Does price sensitivity differ by region?

Customers in Las Vegas and Miami are more sensitive to price changes than those in Washington DC.

Interaction effects show Las Vegas customers exhibit the highest price sensitivity.

![image](https://github.com/user-attachments/assets/9fe973f2-da02-4132-98a4-2735efacc4b0)


### 3. Does price sensitivity vary by income group?

Higher-income customers ($85K+) are less price-sensitive, showing a smaller drop in booking probability.

Lower-income customers (<$40K) are the most price-sensitive, reinforcing prior assumptions about price elasticity.

![image](https://github.com/user-attachments/assets/63af21b3-ca2f-411f-947d-de42f36dbc75)


## Conclusion

This study confirms that experimentally derived price sensitivity estimates are lower than prior observational estimates. While price significantly affects booking decisions, the impact varies by region and income.

## Recommendations

Adjust pricing strategies based on region-specific elasticity.

Consider personalized discounts for price-sensitive customer segments.

Conduct further experiments to refine pricing models for better revenue optimization.

