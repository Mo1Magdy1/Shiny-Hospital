# 🧭 Phase 6 – Prescriptive Analysis

## 📌 Overview
This phase goes beyond prediction — it focuses on **recommendations** and **actionable strategies** derived from the data.  
Using patient admission and discharge data, we identify **optimal resource allocation**, **capacity planning**, and **policy improvements** to enhance healthcare operations.

---

## 🎯 Objectives
1. **Optimal Doctor Allocation per Month**
   - Assign the right number of doctors each month based on patient volume.
   - Minimize patient wait times while maintaining an **ideal ratio of 15 patients per doctor**.

2. **Discharge Policy Recommendations**
   - Identify hospitals and conditions with **excessive Length of Stay (LOS)**.
   - Recommend targeted **discharge planning** to improve patient flow and reduce overcrowding.

3. **Cancer Ward Capacity Optimization**
   - Predict monthly peaks in cancer admissions.
   - Recommend **minimum ward capacity with a 20% buffer** to prevent overflow.

---

## 🛠 Methods & Steps

### **Problem 1: Optimal Doctor Allocation**
- Convert **Date of Admission** to `datetime`.
- Aggregate patients per `YearMonth`.
- Calculate required doctors as:  
  \[
  \text{Required Doctors} = \lceil \frac{\text{Patient Count}}{15} \rceil
  \]
- Output: Month-by-month **required doctor count**.

---

### **Problem 2: Discharge Policy Recommendations**
- Calculate **Length of Stay (LOS)** as:  
  \[
  LOS = \text{Discharge Date} - \text{Date of Admission}
  \]
- Group by **Hospital** and **Medical Condition**.
- Flag hospitals with LOS above the **75th percentile**.
- Output: Table of average LOS per hospital/condition, with **High_LOS_Flag** indicator.

---

### **Problem 3: Cancer Ward Capacity Planning**
- Filter data for `Medical Condition = "Cancer"`.
- Aggregate **monthly admissions**.
- Apply **20% capacity buffer**:
  \[
  \text{Recommended Capacity} = \lceil \text{Cancer Patients} \times 1.2 \rceil
  \]
- Output: Month-by-month **recommended ward capacity**.

---

## 📂 Deliverables
Folder:  

