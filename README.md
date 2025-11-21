# Yulu – Hypothesis Testing for Mobility Service Optimization

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)  
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange)  
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-yellow)  
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-blue)  
![SciPy](https://img.shields.io/badge/SciPy-Statistical%20Testing-purple)  
![Statsmodels](https://img.shields.io/badge/Statsmodels-Regression%20%26%20Inference-teal)  
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-red)  
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Graphics-coral)  
![Hypothesis Testing](https://img.shields.io/badge/Hypothesis%20Testing-A%2FB%20Testing%2C%20Inference-brown)  
![Urban Mobility](https://img.shields.io/badge/Urban%20Mobility-Micro%20Mobility%20Analytics-crimson)

---

## Overview
This project conducts **statistical hypothesis testing** on ride data from **Yulu**, India’s leading micro-mobility startup offering electric bikes and scooters for urban commutes. The goal is to use data-driven inference to evaluate business hypotheses related to user behavior, pricing experiments, and operational performance.

## Problem Statement
Yulu aims to make evidence-based decisions on critical questions such as:
- Did a new **pricing strategy** significantly change average ride duration?  
- Is there a **difference in usage** between weekdays and weekends?  
- Do users in **Bangalore vs. Mumbai** exhibit significantly different riding patterns?  
- Has a recent **app update** led to an increase in daily active users?

To avoid decisions based on anecdotal evidence or random fluctuations, **rigorous hypothesis testing** is applied to validate or reject these business assumptions.

## Solution Approach
This notebook implements a structured **hypothesis testing framework**, including:
- Formulating **null (H₀) and alternative (H₁) hypotheses**  
- Selecting appropriate statistical tests (t-test, z-test, chi-square, ANOVA)  
- Checking **assumptions** (normality, homogeneity of variance, independence)  
- Calculating **p-values** and interpreting results at a significance level (α = 0.05)  
- Computing **effect sizes** to assess practical significance  
- Visualizing distributions and test outcomes for stakeholder communication  

The analysis covers both **one-sample**, **two-sample**, and **proportion-based** tests using real-world micro-mobility metrics.

## Project Structure
```
yulu-hypothesis-testing/
├── Project 5 - Business Case - Yulu - Hypothesis Testing.ipynb  # Main analysis notebook
├── data/
│   └── yulu_rides.csv                     # Anonymized ride-level dataset (timestamp, city, duration, user type, etc.)
├── README.md                              # This documentation
└── requirements.txt                       # Python dependencies
```

## Key Hypothesis Tests Performed
- **Two-sample t-test**: Comparing average ride duration before vs. after a pricing change  
- **Chi-square test of independence**: Testing association between city and user type (new vs. returning)  
- **One-sample z-test**: Verifying if mean daily rides exceed a business target  
- **Proportion test**: Assessing if weekend conversion rate differs from weekday baseline  
- **ANOVA**: Evaluating ride frequency across multiple cities simultaneously  

## Technical Requirements
- Python 3.8+  
- Jupyter Notebook  
- Core libraries:
  - pandas
  - numpy
  - scipy.stats
  - statsmodels
  - matplotlib
  - seaborn

## Installation
1. Clone or download the project  
2. Install required packages:  
   ```bash
   pip install -r requirements.txt
   ```
3. Launch Jupyter:  
   ```bash
   jupyter notebook
   ```

## Usage
1. Open `Project 5 - Business Case - Yulu - Hypothesis Testing.ipynb`  
2. Execute cells sequentially to:  
   - Load and explore the ride dataset  
   - Define business hypotheses  
   - Perform statistical tests with assumption checks  
   - Interpret p-values and effect sizes  
   - Generate visual summaries (histograms, boxplots, bar charts)  

Each test includes clear **business interpretation**—not just statistical significance, but **actionable insights**.

## Business Impact
- Enables **confident decision-making** in product and pricing experiments  
- Reduces risk of **false conclusions** from observed data patterns  
- Supports **A/B testing culture** across marketing, product, and operations teams  
- Provides a **reproducible framework** for future data-driven evaluations  

## Ethical & Practical Notes
- All user data is anonymized and aggregated  
- Statistical significance ≠ business significance—effect size and cost-benefit are emphasized  
- Tests assume proper experimental design (e.g., randomization in A/B tests)

## License
This project is for educational and illustrative purposes only. Data is synthetic or anonymized. Not intended for operational use without proper experimental governance.

---

*Developed as part of a data-driven decision-making case study*  
*Last updated: November 2025*
