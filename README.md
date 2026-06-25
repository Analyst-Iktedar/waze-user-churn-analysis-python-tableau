# Waze User Churn Analysis

A data analytics project focused on understanding and preventing monthly user churn on the Waze navigation app.

---

## Project Overview

This project was developed by the Waze data team with the goal of **increasing overall growth by reducing user churn**. For the purposes of this analysis, churn is defined as users who have either uninstalled the Waze app or stopped using it within a given month.

---

## Objective

Inspect user behavioural data to identify meaningful relationships between variables that may explain why users churn, and use those insights to guide further analysis and predictive modelling.

---

## Dataset

| Property | Details |
|---|---|
| Total Variables | 12 (objects, floats, integers) |
| Class Split | 82% Retained / 18% Churned |
| Missing Values | 700 missing values in the `label` column (possibly non-random) |

---

## Key Findings

- **Churned users drove more frequently** — averaging ~3 more drives per month than retained users.
- **Retained users were more consistent** — they used the app on over twice as many days as churned users in the last month.
- **Churned users covered more ground** — the median churned user drove ~200 more kilometres and logged 2.5 more hours than the median retained user.
- **Churned users show a "super-driver" profile** — more drives, in fewer days, with farther and longer individual trips.
- **Extreme per-day distance** — the median churned user drove **608 km per drive day**, nearly 250% the per-drive-day distance of retained users.
- **Dataset caveat** — regardless of churn status, the users in this dataset are heavy drivers. This data likely does not represent the typical driver population at large.

---

## Methods

1. **Built a structured dataframe** — each row represents a single user observation; each column represents a single variable.
2. **Collected preliminary statistics** — computed summary statistics across all variables for retained vs. churned users.
3. **Analysed user behaviour** — compared driving patterns, app usage frequency, and trip characteristics by churn status.

---

## Insights & Interpretation

Churned users appear to form a distinct behavioural cluster — high-mileage, infrequent-day drivers whose usage pattern differs significantly from retained users. This raises an important hypothesis: **the needs of "super-drivers" may not be well-served by the current Waze experience**, which could be a key driver of churn in this segment.

---

## Next Steps

- [ ] **Gather more data on super-drivers** — understand whether their heavy driving behaviour is also the factor that causes the app to fall short of their needs.
- [ ] **Conduct thorough Exploratory Data Analysis (EDA)** — go beyond summary statistics to uncover deeper patterns.
- [ ] **Develop data visualisations** — build charts and dashboards to illustrate the narrative behind the data and communicate findings to stakeholders.
- [ ] **Address missing label values** — investigate whether the 700 missing values in the `label` column are missing at random (MAR) or systematically missing, as this will affect modelling decisions.

---

## Project Status

> **Milestone 2 — Preliminary Data Summary: Complete**
>
> The team has identified important relationships between variables. The immediate next phase is full EDA and visualisation development.

---

## Prepared For

**Waze Leadership Team**

---

*This README is based on the Milestone 2 Preliminary Data Summary report.*
