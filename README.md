# 🏥 Hospital Emergency Room Analytics Dashboard

## 1. Project Title / Headline

### 🏥 Hospital Emergency Room Analysis: Interactive Excel Dashboard

An interactive hospital emergency room dashboard developed to analyze patient visits, waiting time, satisfaction scores, admission status, patient demographics, and department referrals.

---

## 2. Short Description / Purpose

The Hospital Emergency Room Dashboard provides an interactive view of emergency room performance and patient-related metrics.

The dashboard helps analyze patient volume, average waiting time, patient satisfaction, admission status, timeliness of service, gender distribution, age groups, and department referrals.

The main objective is to convert hospital emergency room data into meaningful visual insights that can help stakeholders monitor performance and identify areas requiring attention.

---

## 3. Tech Stack

The dashboard was developed using:

- 📊 **Microsoft Excel** – Dashboard development and visualization
- 🔄 **Power Query** – Data import, cleaning, and transformation
- 🧮 **Power Pivot** – Data modeling and analysis
- 📐 **DAX** – Calculated columns and analytical calculations
- 📅 **Calendar Table** – Time-based analysis
- 📈 **Pivot Tables & Charts** – Data summarization and visualization

---

## 4. Data

The project uses hospital emergency room data containing information related to:

- Patient visits
- Patient age
- Gender
- Waiting time
- Admission status
- Patient satisfaction score
- Department referrals
- Patient attendance status
- Date and time information

The dashboard supports analysis across different months and years.

---

# 5. Business Problem

Hospital emergency room data contains information about patients, waiting times, admissions, satisfaction, and referrals.

Analyzing this information manually can make it difficult to identify important patterns and monitor emergency room performance.

The dashboard was developed to answer questions such as:

- How many patients visited the emergency room?
- What is the average patient waiting time?
- How satisfied are the patients?
- How many patients were admitted?
- How many patients were attended within the expected time?
- What is the patient distribution by age and gender?
- Which departments receive the most patient referrals?

---

# 6. Dashboard Objectives

The main objectives of the dashboard are:

- Monitor the number of emergency room patients.
- Track average patient waiting time.
- Analyze patient satisfaction scores.
- Compare admitted and non-admitted patients.
- Analyze patient attendance timeliness.
- Understand patient demographics.
- Analyze department referral patterns.
- Provide monthly and yearly performance analysis.

---

# 7. Dashboard Features / Highlights

## 🔹 KPI Analysis

The dashboard includes important KPIs such as:

- **Number of Patients**
- **Average Wait Time**
- **Patient Satisfaction Score**

The KPIs provide a quick overview of emergency room performance.

---

## 🔹 Patient Admission Analysis

The dashboard compares:

- Admitted patients
- Not admitted patients

It also displays the percentage contribution of each admission status.

---

## 🔹 Patient Age Analysis

Patients are grouped into different age categories:

- 0–4
- 05–14
- 15–29
- 30–44
- 45–59
- 60–69
- 70–79

This helps understand the age distribution of emergency room visitors.

---

## 🔹 Timeliness Analysis

Patient attendance is categorized into:

- **Within Time**
- **Delay**

The dashboard visualizes the proportion of patients attended within the expected time.

---

## 🔹 Gender Analysis

A donut chart displays the number of patients by gender.

This provides a quick view of the gender distribution of emergency room visitors.

---

## 🔹 Department Referral Analysis

The dashboard shows the number of patients referred to different departments.

Departments displayed include:

- General Practice
- Orthopedics
- Physiotherapy
- Gastroenterology
- Cardiology
- Neurology
- Renal

This helps identify departments receiving higher numbers of referrals.

---

## 🔹 Monthly Analysis

Users can select different months using the dashboard navigation.

The dashboard can therefore be used to analyze emergency room performance for different monthly periods.

---

# 8. Data Preparation & Modeling

The project followed an end-to-end data analytics workflow:

1. Business requirement gathering
2. Understanding the data
3. Data connection using Power Query
4. Data cleaning and quality checks
5. Calendar table creation
6. Data modeling using Power Pivot
7. Creation of calculated columns using DAX
8. Pivot table creation
9. Dashboard layout development
10. Chart development and formatting
11. Dashboard development
12. Insight generation

This workflow is documented in the project presentation. :contentReference[oaicite:1]{index=1}

---
#Screenshort:
(https://github.com/pegurohim1-0304/Excel-Project/blob/main/Hospital%20Dashboard%20Final%20.jpg)


# 9. DAX & Analytical Calculations

### Age Group Classification

A DAX calculation was used to classify patients into different age groups.

```DAX
=IF([Patient Age]>=70,"70-79",
IF([Patient Age]>=60,"60-69",
IF([Patient Age]>=45,"45-59",
IF([Patient Age]>=30,"30-44",
IF([Patient Age]>=15,"15-29",
IF([Patient Age]>=5,"05-14","0-4"))))))

