# Hospital Management System Analysis using MySQL

## Overview

This project analyzes a Hospital Management System database using MySQL. The dataset contains information about patients, doctors, departments, diagnoses, treatments, payment methods and hospital visits. The objective of the project is to perform healthcare analytics and generate business insights using advanced SQL concepts such as joins, aggregations, CTEs, window functions, ranking functions and date-based analysis.

---

## Dataset Size

The project is built on a dataset containing more than **16,000 hospital visit records** along with supporting dimension tables.

| Table            | Records |
| ---------------- | ------: |
| Patient_Visits   |  16,640 |
| Patient          |   2,436 |
| Patient_Clean    |   2,431 |
| Doctor           |     200 |
| Department       |      40 |
| Department_Clean |      33 |
| Diagnosis        |      40 |
| Treatment        |      30 |
| PaymentMethod    |       4 |

### Historical Visit Data

| Table                   | Records |
| ----------------------- | ------: |
| PatientVisits_2020_2021 |   7,084 |
| PatientVisits_2022_2023 |   5,011 |
| PatientVisits_2024      |   2,987 |
| PatientVisits_2025      |   1,313 |

**Total Records Across All Tables: ~38,000+**

---

## Database Schema

The database consists of the following entities:

### Fact Table

* Patient_Visits

### Dimension Tables

* Patient
* Doctor
* Department
* Diagnosis
* Treatment
* PaymentMethod

A cleaned version of selected tables was also created during the data-cleaning phase:

* Patient_Clean
* Department_Clean

---

## SQL Concepts Used

* INNER JOINs
* Aggregate Functions
* Common Table Expressions (CTEs)
* Window Functions
* Ranking Functions
* CASE Expressions
* Date Functions
* String Functions
* Running Totals
* Data Cleaning Techniques
* Business Intelligence Queries

---

## Data Cleaning Performed

### Patient Table

* Standardized patient names
* Expanded gender abbreviations
* Split location information into:

  * City
  * State
  * Country

### Department Table

* Removed records with missing department categories
* Dropped unnecessary columns
* Standardized department naming using specialization information

---

## Analysis Performed

### Doctor Analytics

* Counted distinct patients treated by each doctor
* Identified doctors with the highest average satisfaction score (minimum 100 visits)

### Revenue Analytics

* Revenue split by payment method
* Department-wise revenue analysis
* Department ranking based on revenue generation

### Patient Analytics

* Age-group based billing analysis
* Patient satisfaction analysis
* Visit frequency analysis

### Department Analytics

* Average satisfaction score by department
* Average waiting time by department
* Revenue comparison across departments

### Hospital Operations Analytics

* Weekday vs weekend visit comparison
* Monthly visit trends
* Running cumulative visit analysis

### Diagnosis & Treatment Analytics

* Most commonly prescribed treatment for each diagnosis

---

## Key Business Questions Answered

* Which doctors treat the highest number of unique patients?
* Which payment methods generate the highest revenue?
* Which age groups incur the highest average hospital bills?
* Which departments generate the most revenue?
* How do departments rank within their category?
* Which departments provide the best patient experience?
* How do visit patterns differ between weekdays and weekends?
* How have hospital visits changed over time?
* Which treatments are most commonly prescribed for specific diagnoses?

---

## Technologies Used

* MySQL Workbench
* SQL Window Functions
* SQL CTEs

---

## Author
Afreen S

