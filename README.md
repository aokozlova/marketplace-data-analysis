# Marketplace Retention and Growth Analysis

This project analyses customer behaviour and performance metrics of an e-commerce marketplace.
The goal is to find why revenue growth has stalled, identify product–market fit issues, and propose data-driven hypotheses for improvement.

## Overview

* Dataset: anonymised marketplace data (orders, customers, items)
* Period: 2017–2018
* Tools: Python (pandas, matplotlib, seaborn)
* Focus: retention, product–market fit, key growth metrics, hypothesis prioritisation with ICE framework

## Key Steps

1. Data Preparation
    - Merged customer, order, and item datasets
    - Checked data consistency and missing values
    - Found anomalies in delivery and approval timestamps
2. Retention Analysis
     - Calculated monthly retention based on delivered orders
     - Built a cohort heatmap
     - Median 1st-month retention: 0.35%
> !!!!! RETENTION HEATMAP

3. Product–Market Fit
    - Only 3% of customers made more than one purchase
    - Retention declines across cohorts

**Conclusion: no product–market fit yet**.Customers don’t return after the first purchase
> !!!!!!!!!RETURN RATE CHART

4. Performance Metrics
Defined key metrics to track marketplace growth:
    - Gross Merchandise Value
    - Monthly Active Users
    - Repeat Customer Rate
    - Average Revenue Per Paying User

> !!!!!! LINE CHARTS

5. Hypothesis Testing (ICE Framework)
Three improvement hypotheses were evaluated:
<br>

> H1: Fix order processing bug → fewer cancellations
> H2: Shorten shipping time → fewer delays, more repeat orders
> H3: Add new payment option → easier checkout, more repeat customers

H1 received the highest ICE score (192 points) and was selected for A/B testing.
> !!!!! ICE TABLE

6. A/B Test Design
    - **Target metric:** Delivery Rate
    - **Proxy metric:** Pick-Up Rate
    - **Guardrail metric:** Order Conversion Rate

## Findings

* Retention and repeat activity are critically low (only 3% of users return).

* The marketplace hasn’t reached product–market fit.

* 8.5% of orders were delayed, and ~1,300 orders had inconsistent timestamps.

* Order processing issues likely block deliveries and lower retention.

## Next Steps
* Run the A/B test for Hypothesis 1 (order processing fix).
* Monitor Pick-Up Rate and Delivery Rate as key indicators.
* Explore new hypotheses for user reactivation and loyalty improvement.
