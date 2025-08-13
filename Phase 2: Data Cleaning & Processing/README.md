# 🏥 Patient Admission Data Analysis – Phase 2: Data Cleaning & Processing

This is **Phase 2** of a multi-stage hospital data analysis project.  
In this phase, we focus on **Data Cleaning and Processing** to ensure the dataset is consistent, reliable, and ready for statistical analysis and modeling in later stages.

> **Note:** This project is implemented in **Python**, **R**, and **SQL**.  
> All three implementations follow the same Phase 2 steps to produce identical cleaned datasets.

---

## 🎯 Objectives
- Normalize and standardize data for consistency.
- Detect and handle missing or invalid entries.
- Remove duplicate records.
- Standardize categorical values (e.g., gender).
- Format date fields for accurate calculations.
- Prepare a cleaned dataset with selected relevant variables.

---

## 📂 Dataset
**File:** `patients.xlsx`  
**Key Columns:**
- `Name`, `Doctor` — Full patient and doctor names.
- `Age`, `Gender`, `Blood Type`, `Medical Condition` — Demographic and health information.
- `Date of Admission`, `Discharge Date` — Hospitalization dates.
- `Insurance Provider`, `Billing Amount`, `Room Number` — Administrative data.
- `Admission Type`, `Medication`, `Test Results` — Clinical data.

---

## 🔍 Cleaning Steps in Phase 2
1. **Name Normalization**
   - Split full names into `First_Name` and `Last_Name`.
   - Capitalize names properly.
   - Remove titles like "Dr.", "Mr.", "Miss".
2. **Doctor Name Normalization**
   - Apply same cleaning process as for patients.
3. **Missing & Invalid Data Detection**
   - Identify rows with null or invalid entries in key fields (e.g., missing age, billing amount ≤ 0).
4. **Duplicate Removal**
   - Remove duplicate records based on patient name and date of admission.
5. **Gender Standardization**
   - Convert variations like `m`, `male`, `man` to `Male`; `f`, `female`, `woman` to `Female`.
6. **Date Conversion**
   - Convert admission and discharge dates to proper datetime format.
7. **Analysis Table Creation**
   - Select only relevant cleaned columns for further analysis.

---

## 📈 Results
- All patient and doctor names are standardized.
- Missing or invalid entries have been flagged for review.
- Duplicate patient admissions are removed.
- Gender values are fully standardized to `Male` or `Female`.
- Dates are uniformly formatted and ready for time-based calculations.
- A final **analysis table** with 17 cleaned columns is generated for downstream analysis.

---

## 🛠️ Requirements
**Python:**
- pandas, numpy, re (built-in), openpyxl, datetime, dateutil

**R:**
- tidyverse, lubridate, readxl, stringr, dplyr

**SQL:**
- Standard SQL string manipulation and date functions  
- Requires patient data imported into a database table


