# Hospital Analytics Dashboard (Power BI)
<p align="center">
  <img src="https://github.com/user-attachments/assets/bfbc9cd9-ff24-438d-b2d4-6466317bfbb4" width="100%" alt="Hospital Analytics Dashboard Banner">
</p>

<h1 align="center">🏥 Hospital Analytics Dashboard</h1>

<p align="center">
Interactive Power BI dashboard for analyzing hospital operations, admissions, revenue, clinical efficiency, and patient demographics.
</p>

<p align="center">

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-Data%20Analysis-blue?style=for-the-badge)
![Power Query](https://img.shields.io/badge/Power_Query-ETL-success?style=for-the-badge)
![Apache 2.0](https://img.shields.io/badge/License-Apache_2.0-green?style=for-the-badge)

</p>

<p align="center">
Interactive Power BI dashboard for analyzing hospital operations, admissions, revenue, clinical efficiency, and patient demographics.
</p>

An interactive 4-page Power BI dashboard analyzing hospital operations across admissions, revenue, clinical efficiency, patient demographics, and doctor performance. Built on a synthetic healthcare dataset of ~55,500 patient records.

## Overview

A single reporting solution for hospital administrators to monitor financial performance, patient throughput, clinical efficiency, and provider workload. The report is split into four role-focused pages, so executives, clinicians, and operations staff each get the view relevant to them. Every page is filterable by hospital and year, with cross-filtering across all visuals.

## Preview
<img width="1153" height="642" alt="image" src="https://github.com/user-attachments/assets/440a6b7c-8baf-4d9d-af72-49996ce670c4" />
<img width="1153" height="647" alt="image" src="https://github.com/user-attachments/assets/28e410e3-3490-4a79-8f1b-2a7ae9e70ea4" />
<img width="1157" height="653" alt="image" src="https://github.com/user-attachments/assets/f9c5cf10-7f28-49e7-9a49-1099347749ae" />
<img width="1158" height="647" alt="image" src="https://github.com/user-attachments/assets/f20e8e23-980c-42ea-81fb-0bd1d45a28c6" />




## Report Pages

### 1. Executive
High-level financial and admissions KPIs for leadership.

- **KPI cards:** Total Admissions (55.5K), Total Revenue (1.42bn), Average Billing Amount (25.54K), Average Stay (15.51 days)
- Total Revenue and Total Admissions by month (combined column and line)
- Total Revenue by Medical Condition (Diabetes, Obesity, Arthritis, Hypertension, and others)
- Total Admissions by Admission Type (Elective 49.95%, Emergency 33.28%, Urgent 16.77%)
- Total Revenue by Insurance Provider (Cigna, UnitedHealthcare, Medicare, Blue Cross, Aetna)

### 2. Clinical Operations and Efficiency
Operational efficiency across hospitals, stay length, and admission types.

- **KPI cards:** Total Patients Treated (37K), Average Patient Stay (15.52 days), Emergency Caseload (37K)
- Total Revenue and Total Admissions by Hospital
- Impact of Admission Type on Stay and Billing (matrix: average length of stay and average billing amount per admission type)
- Total Admissions by month and admission type (line)
- Length of Stay Distribution (histogram, 0 to 30 days)

### 3. Patient Demographics
Patient population profile by age, gender, blood type, and condition.

- **KPI cards:** Total Patients (56K), Average Patient Age (51.51), Most Common Blood Type (A-)
- Total Admissions by Medical Condition and Gender (100% stacked bar)
- Age Distribution (histogram)
- Total Admissions by Blood Type (treemap)
- Revenue by Gender and Admission Type (matrix)

### 4. Doctor and Provider Performance
Provider-level workload, revenue, and insurance mix.

- **KPI cards:** Total Doctors, Total Patients Treated (56K), Total Revenue (1.42bn)
- Total Revenue and Total Admissions by Doctor (combined column and line)
- Total Revenue by Insurance Provider (donut: Cigna, UnitedHealthcare, Medicare, Blue Cross, Aetna)
- Top 5 Doctors: Caseload and Revenue (matrix broken down by admission type)

## Data

- **Source:** [Healthcare Dataset on Kaggle](https://www.kaggle.com/datasets/prasad22/healthcare-dataset)
- **Records:** ~55,500 rows
- **Key fields:** Age, Gender, Blood Type, Medical Condition, Date of Admission, Doctor, Hospital, Insurance Provider, Billing Amount, Room Number, Admission Type, Discharge Date, Medication, Test Results
- **Note:** This is a synthetic dataset. It contains no real patient information.

## Tools and Techniques

- Power BI Desktop
- Power Query for data cleaning and transformation (ETL)
- DAX measures for KPIs (Total Revenue, Average Stay, Average Billing Amount, Emergency Caseload, admission percentages)
- Star schema data model
- Interactive slicers (Hospital Name, Year) with cross-filtering across all visuals
- Page navigation buttons for a multi-view report experience
- Matrix visuals, treemaps, histograms, and combined column-and-line charts

## How to Use

1. Download `dashboard/Hospital_Analytics.pbix`
2. Open it in Power BI Desktop (free)
3. Use the Hospital Name and Year slicers to filter, and the top navigation buttons to switch between the four pages

## Author

**Huzaima** - Data Science student at COMSATS University Islamabad

[https://www.linkedin.com/in/huzaima-imtiaz/](#) 
