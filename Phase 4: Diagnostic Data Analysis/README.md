# 📊 Phase 4 – Diagnostic Data Analysis

## 📌 Overview
This phase focuses on **diagnostic analysis** of the patient admission dataset.  
The aim is to evaluate **data integrity, statistical assumptions, and variable relationships** before moving to advanced modeling.  


> **Note:** This phase contains code in **Python**, **R**, and **SQL** to ensure reproducibility across platforms.

---

## 🎯 Goals
- Perform **univariate** and **bivariate** diagnostic checks.
- Identify **outliers** using boxplots, leverage plots, and influence statistics.
- Check **normality** assumptions for continuous variables.
- Evaluate **multicollinearity** using Variance Inflation Factor (VIF).
- Explore **categorical vs. categorical** relationships with Chi-square and Cramer’s V.
- Explore **continuous vs. continuous** relationships with Pearson correlation.
- Conduct **cohort analysis** to monitor patient behavior over defined periods.
- Perform **time series analysis** to reveal seasonality and trends.
- Identify **non-parametric differences** using Mann–Whitney U tests.

---

## 🛠 Methods
- **Python:** `pandas`, `numpy`, `scipy.stats`, `statsmodels`, `matplotlib`, `seaborn`
- **R:** Equivalent statistical tests and plots implemented
- **SQL:** Data selection and filtering for diagnostic subsets

---

## 🔍 Key Analyses
1. **Outlier Detection**
   - Boxplots
   - Leverage plots
   - Influence plots

2. **Correlation Analysis**
   - Pearson’s correlation (continuous variables)
   - Cramer’s V (categorical variables)

3. **Normality & Distribution**
   - Histograms with density curves
   - Shapiro–Wilk and Kolmogorov–Smirnov tests

4. **Multicollinearity**
   - Variance Inflation Factor (VIF)

5. **Cohort Analysis**
   - Grouping patients by admission month/year
   - Tracking patient flow and readmissions over time

6. **Time Series Analysis**
   - Aggregating admissions and billing amounts by time
   - Identifying trends, seasonality, and anomalies

7. **Group Comparisons**
   - t-tests (parametric)
   - Mann–Whitney U tests (non-parametric)

---

## 📈 Visualization
📂 **See the `visualizations/phase4` folder** for:
- Correlation heatmaps
- Outlier boxplots
- Leverage and influence plots
- Cohort retention charts
- Time series plots

---

