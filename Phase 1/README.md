# 🏥 Patient Admission Data Analysis – Phase 1: Data Exploration

This is **Phase 1** of a multi-stage hospital data analysis project.  
In this phase, we focus on **Exploratory Data Analysis (EDA)** to understand the dataset, identify key patterns, and prepare for deeper statistical and predictive modeling in later phases.

> **Note:** This project is implemented in **Python**, **R**, and **SQL**.  
> All three versions perform the same Phase 1 tasks so results are consistent across programming environments.

---

## 🎯 Objectives
- Inspect and understand the structure of the dataset.
- Summarize demographic and medical information about patients.
- Calculate descriptive statistics for age, hospital stays, and billing amounts.
- Identify unusual or extreme values (negative bills, small bills).
- Explore distributions of categorical variables such as gender, blood type, and admission type.

---

## 📂 Dataset
**File:** `patients.xlsx`  
**Key Columns:**
- `Gender` — Patient gender.
- `Age` — Age at admission.
- `Insurance Provider` — Insurance company name.
- `Blood Type` — Blood group.
- `Medical Condition` — Primary diagnosis/condition.
- `Admission Type` — Emergency, elective, etc.
- `Doctor` — Attending physician.
- `Hospital` — Hospital name.
- `Date of Admission` — Admission date.
- `Discharge Date` — Discharge date.
- `Billing Amount` — Patient billing total.

---

## 🔍 Analysis Steps in Phase 1
1. **Data Loading & Setup**
   - Import necessary Python, R, or SQL environment.
   - Load the dataset.
2. **Basic Exploration**
   - Display top 10 rows.
   - Identify unique values for categorical fields.
3. **Demographic Statistics**
   - Maximum, minimum, mean, and median patient ages.
4. **Hospital Resource Statistics**
   - Number of unique doctors and hospitals.
5. **Date Analysis**
   - Earliest and latest admission/discharge dates.
   - Calculate date differences (years, months, days).
6. **Length of Stay (LOS)**
   - Calculate average, maximum, and minimum LOS in days.
7. **Billing Analysis**
   - Minimum, maximum, mean, and range of billing amounts.
   - Detect negative bills and very small bills ($0–$50).

---

## 📈 Key Findings
- Clear age distribution range with calculated average and median values.
- Variation in hospital stay lengths, with outlier detection.
- Detection of abnormal financial entries (negative and low-value bills).
- Identification of diversity in admission types, medical conditions, and insurance providers.

---

## 🛠️ Requirements
**Python:**
- Python ≥ 3.9
- pandas, numpy, seaborn, matplotlib, scipy, python-dateutil, openpyxl, statsmodels, prophet

**R:**
- tidyverse, lubridate, readxl, dplyr, ggplot2, summarytools

**SQL:**
- Works with standard SQL (tested on PostgreSQL & MySQL)
- Requires import of `patients.xlsx` into a database table before running queries



