# A/B Test Simulation and Analysis

This project demonstrates the simulation, analysis, and statistical testing of an A/B test using Python. It generates mock user-level data for control and treatment groups, calculates conversion rates, performs hypothesis testing, and computes required sample size for a given power.

---

## Project Overview

- **Data Generation**: Simulates an A/B test dataset with 10,000 users split evenly between control and treatment groups.
- **Metrics Simulated**:
  - User ID
  - Group assignment (Control vs Treatment)
  - Date of interaction (randomized within a 14-day test period)
  - Page Views
  - Clicks (constrained to be ≤ Page Views)
  - Conversion indicator (binary outcome)
- **Conversion Rates**:
  - Control group baseline conversion: 10%
  - Treatment group with a slight uplift: 11.5%
- **Analysis Steps**:
  - Check for duplicate users across groups and missing values
  - Summary statistics and boxplots for page views and clicks
  - Calculate conversion rates per group
  - Perform a two-sided z-test for conversion rate difference
  - Calculate 95% confidence intervals for conversion rates
  - Compute required sample size for detecting a 1.5% uplift with 80% power

---

## Files

- `ab_test_results_mock_data.csv` : The simulated A/B test dataset.
- `ab_test_analysis.py` : Python script containing data generation, analysis, and statistical testing.
---


