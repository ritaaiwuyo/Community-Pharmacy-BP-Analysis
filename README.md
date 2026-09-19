# Community Pharmacy Blood Pressure Analysis

## Project Overview

This project analyses real-world, de-identified blood pressure data collected during routine community pharmacy practice.

The analysis explores blood pressure patterns across patient encounters, demographic characteristics, patient follow-up, and changes in blood pressure between baseline and the latest recorded follow-up.

The project demonstrates how routinely collected community pharmacy data can be transformed into meaningful clinical and public health insights using Excel and Power BI.

## Dataset

- 381 blood pressure encounters
- 140 unique patients
- 63 returning patients
- Real-world community pharmacy data
- Patient identifiers and actual visit dates removed before analysis

Repeat visits were intentionally retained to support longitudinal analysis.

> **Privacy Note:** The underlying patient-level dataset is not publicly shared. Only aggregated, de-identified analytical outputs are presented in this repository.

## Tools Used

- Microsoft Excel - data cleaning, validation and de-identification
- Power Query - data transformation and preparation
- Power BI - data modelling, DAX measures, analysis and dashboard development
- DAX - KPI calculations and longitudinal patient-level analysis

## Methodology

Blood pressure readings were classified using JNC 7 categories: Normal, Prehypertension, Stage 1 Hypertension and Stage 2 Hypertension. Where systolic and diastolic readings fell into different categories, the higher category was assigned.

For longitudinal analysis, multiple BP readings recorded for the same patient on the same follow-up day were averaged. Baseline BP was based on Day 0 readings, while latest BP represented the patient's most recent recorded follow-up day.

Follow-up BP status was classified as:

- **Improved:** latest BP category was lower than baseline
- **Unchanged:** latest BP category remained the same
- **Worsened:** latest BP category was higher than baseline

## Key Findings

- 43.6% of recorded BP encounters were within the hypertensive range (Stage 1 or Stage 2).
- 63 of 140 patients (45.0%) returned for at least one follow-up BP assessment.
- Adults aged 50–59 years were the largest patient group, accounting for 47 of 140 patients (33.6%).
- Prehypertension was the most frequently recorded BP category with 134 encounters, followed by Stage 1 hypertension with 117 encounters.
- Among returning patients, 18 (28.6%) moved to a lower BP category, 30 (47.6%) remained unchanged, and 15 (23.8%) moved to a higher category.
- Average BP among returning patients changed from 131.4/83.2 mmHg at baseline to 126.7/81.1 mmHg at the latest recorded follow-up.

## Dashboard

The Power BI report contains two analytical pages:

### 1. BP & Patient Overview
Provides an overview of patient demographics, BP classifications, encounter patterns and follow-up participation.

### 2. Follow-up & BP Change
Examines longitudinal BP changes among returning patients, including baseline-to-latest BP comparison and follow-up status by sex.

## Important Interpretation Note

This is an observational analysis of routinely collected community pharmacy data. Changes in BP during follow-up should not be interpreted as evidence of treatment effectiveness or medication effect because information on adherence, medication dose, treatment duration, comorbidities and other potential explanatory factors was not available.

## Author

**Dr. Rita Aiwuyo, PharmD, R.Ph**  
Licensed Pharmacist | Healthcare Data Analyst | Public Health Professional
