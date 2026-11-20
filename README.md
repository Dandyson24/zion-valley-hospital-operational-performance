 
# 🏥 Hospital Operational Performance Analysis | Zion Valley Specialist Hospital

### Turning Healthcare Data into Actionable Insights with Power BI

## 📌 Project Overview

How efficiently does a hospital deliver care to its patients?

This project explores patient encounters and waiting-time performance at **Zion Valley Specialist Hospital**, using healthcare data to identify operational patterns, departmental workload variations and potential delays in service delivery.

The objective was to move beyond reporting hospital activity figures and provide management with actionable insights to support operational efficiency and improve patient experience.

The analysis covers **January–December 2025**.

## 🎯 Business Problem

Hospital management received concerns about patient waiting times and changing patient activity across departments. However, there was insufficient evidence to determine whether these concerns represented isolated incidents or broader operational patterns.

The analysis sought to answer five key questions:

1. How is patient activity distributed across hospital departments?
2. How does patient volume change over time?
3. Which departments record the highest average waiting times?
4. How do actual waiting times compare with management-approved targets?
5. Which departments and periods require further operational investigation?

## 📂 Dataset Description

Three CSV datasets were integrated:

| Dataset | Records | Description |
|---|---:|---|
| Encounters | 6,154 | Patient visits, departments, registration and service-start timestamps |
| Patients | 2,600 | Patient demographics, date of birth, sex and payer information |
| Departments | 8 | Department identifiers and classifications |

Two additional analytical tables were created in Power BI:

- Date Table: For time-based analysis and reporting.
- Waiting Time Target Table: For departmental performance benchmarking.

## 🧹 Data Preparation and Cleaning

Data preparation involved:

- Identifying and removing 14 duplicate encounter records.
- Assessing missing service-start timestamps.
- Identifying negative and extreme waiting-time intervals.
- Standardising categorical variables and department identifiers.
- Checking patient and department relationships.
- Converting date and timestamp fields into appropriate formats.
- Creating calculated columns for waiting time, age, age groups and service commencement.

## ⚙️ Tools and Technologies

- **Microsoft Power BI:** Data modelling, DAX calculations, interactive dashboards and visualisation.
- **Power Query:** Data transformation and cleaning.
- **DAX:** Measures, calculated columns and analytical KPIs.
- **CSV:** Source data format.

## 🏗️ Data Modelling and DAX

A relational star-schema approach was adopted, with Encounters serving as the central fact table.

Key calculations included:

| Measure / Calculation | Analytical Purpose |
|---|---|
| Total Encounters | Measures hospital activity |
| Total Unique Patients | Measures unique patients served |
| Registration-to-Service Waiting Time | Calculates patient waiting time in minutes |
| Average Waiting Time | Measures average service commencement delay |
| Service Started | Identifies encounters with recorded service commencement |
| Age | Calculates patient age at latest registration |
| Age Group | Supports demographic segmentation |
| Waiting Time Gap | Measures variance from approved targets |
| Waiting Time Status | Classifies performance against targets |
| LOS and Average LOS | Supplementary inpatient operational measures |

## 📊 Key Findings

### 1. Patient Activity

- 6,140 unique encounters were identified after duplicate removal.
- These encounters involved 2,355 unique patients.
- Outpatient Clinic recorded the highest activity with 1,334 encounters.
- Emergency followed with 1,054 encounters.

### 2. Waiting-Time Performance

The analysis revealed substantial differences between actual average waiting times and approved management targets.

| Department | Actual Average | Approved Target |
|---|---:|---:|
| Emergency | 52.7 minutes | 5 minutes |
| Outpatient Clinic | 51.7 minutes | 15 minutes |

Other departments recorded average waiting times of approximately 28–30 minutes.

### 3. Temporal Patterns

- July recorded the highest patient volume, with 553 encounters.
- February recorded the lowest, with 466 encounters.
- Waiting times fluctuated across the reporting period without a consistent upward or downward trend.

## 💡 Management Recommendations

The analysis identified six priority areas for management attention:

1. Investigate waiting-time variations in Emergency and Outpatient Clinic.
2. Review staffing availability, service capacity and workload distribution.
3. Strengthen patient-flow monitoring from registration to service commencement.
4. Investigate peak activity periods, particularly July.
5. Improve data quality and timestamp documentation.
6. Institutionalise departmental performance monitoring against approved targets.

## ⚠️ Limitations

The analysis identifies operational patterns but cannot independently establish the causes of delays.

Other limitations include:

- Missing service-start timestamps in 60 encounters.
- 15 negative waiting-time intervals requiring validation.
- Three extreme waiting-time records exceeding eight hours, excluded from provisional averages pending verification.
- Fourteen encounters with an unmatched department code (D99).
- The Specialist Clinic target requires confirmation and departmental mapping.
- Available data does not adequately explain staffing constraints, patient acuity or clinical prioritisation.

Consequently, waiting-time differences should be treated as signals for further investigation rather than definitive evidence of poor departmental performance.

## 🚀 Project Impact and Learning Outcomes

This project demonstrates how healthcare data analytics can support hospital management by:

- Converting raw hospital records into meaningful operational KPIs.
- Identifying departmental workload and waiting-time variations.
- Benchmarking operational performance against approved targets.
- Supporting evidence-based management discussions.
- Translating analytical findings into practical recommendations for patient experience improvement.

## 🔑 Key Takeaway

**The objective of healthcare analytics is not merely to count patients, but to understand how efficiently healthcare services are delivered and where improvements can make a meaningful difference to patient experience.**

This project reinforces the role of Business Intelligence in transforming hospital data into actionable operational intelligence.


### 👨‍💻 Author

**Healthcare Data Analytics | Business Intelligence | Public Health**

*Turning Healthcare Data into Actionable Insights.*

#HealthcareAnalytics #PowerBI #DataAnalytics #BusinessIntelligence #HealthcareData #DAX #HospitalPerformance #PatientExperience #DataDrivenHealthcare
