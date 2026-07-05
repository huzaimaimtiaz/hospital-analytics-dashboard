# Hospital Analytics Dashboard (Power BI)

An interactive 4-page Power BI dashboard analyzing hospital operations across admissions, revenue, clinical efficiency, patient demographics, and doctor performance. Built on a synthetic healthcare dataset of ~55,500 patient records.

## Overview

A single reporting solution for hospital administrators to monitor financial performance, patient throughput, clinical efficiency, and provider workload. The report is split into four role-focused pages, so executives, clinicians, and operations staff each get the view relevant to them. Every page is filterable by hospital and year, with cross-filtering across all visuals.

## Preview

![Executive Dashboard](screenshots/executive.png)
![Clinical Operations Dashboard](screenshots/clinical.png)
![Patient Demographics Dashboard](screenshots/demographics.png)
![Doctor and Provider Performance](screenshots/doctor.png)

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

**Huzaima** — Data Science student at COMSATS University Islamabad

[LinkedIn](#) · [Portfolio](#)
