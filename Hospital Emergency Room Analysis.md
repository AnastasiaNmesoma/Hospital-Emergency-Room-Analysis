# **HOSPITAL EMERGENCY ROOM ANALYSIS**

**Project Title:** Hospital Emergency Room Dashboard  
**Tool Used:** Microsoft Power BI (Power Query & DAX)

## **Project Overview**

The goal of this project is to analyze hospital emergency room (ER) operations using patient  
visit data to monitor performance and identify opportunities for operational improvement.

The dataset contains patient records with information such as admission dates, patient demographics, wait times, satisfaction scores, admission status, and department referrals.  
The analysis focuses on:

* Patient volume and daily trends  
* Average patient wait time  
* Patient satisfaction  
* Department referrals  
* Patient demographics  
* Admission patterns

## **Data Preparation**

The dataset was cleaned and transformed before visualization.  
The following data preparation activities were carried out:

* Combined patient first initials and last names into a single Patient Full Name field.  
* Standardized gender values by replacing abbreviated entries (F and M) with their full descriptions (Female and Male).  
* Created a dedicated Date table to support time-based analysis.  
* Added Month and Year fields to enable monthly and yearly reporting.  
* Established a relationship between the Date table and the Hospital ER dataset.

## **Data Modeling**

A star-schema data model was implemented using a centralized Date table linked to the Hospital ER fact table.  
Additional calculated fields were created to support reporting, including:

* Admission Status  
* Age Group  
* Wait Time Status  
* Wait Time Interval  
* Day Name  
* Month/Year

# **Dashboard Structure**

## **Page 1 – Performance Overview**

This page provides a high-level overview of emergency room performance using key performance indicators and interactive visualizations.

### **Key Performance Indicators**

* Number of Patients  
* Average Wait Time  
* Patient Satisfaction Score  
* Number of Patients Referred

Each KPI includes a daily trend visualization to monitor performance over time.

### **Visualizations**

* Patient Admission Status  
* Patients by Age Group  
* Department Referrals  
* Patients Seen Within Target Wait Time  
* Patients by Gender  
* Patients by Race  
* Patient Volume by Day and Time Interval

### **Interactive Filters**

* Year  
* Month/Year

## **Page 2 – Patient Records**

This page provides a detailed view of individual patient records, including:

* Patient ID  
* Patient Name  
* Gender  
* Age  
* Admission Date  
* Race  
* Wait Time  
* Department Referral  
* Admission Status

## **Page 3 – Key Takeaways**

This page summarizes the key findings from the analysis, highlighting trends in patient volume, wait times, satisfaction, referrals, demographics, and admission patterns to support operational decision-making.

### **Key Insights**

#### **Overall Performance**

Between **April 2023 and October 2024**, the emergency room recorded **9,216 unique patient visits**, indicating a consistently high demand for emergency healthcare services throughout the reporting period.

#### **Patient Wait Time & Satisfaction**

The average patient wait time was **35.3 minutes**, exceeding the 30-minute target and suggesting opportunities to improve patient flow. The average satisfaction score of **4.99/10** indicates moderate patient experience, with wait times likely contributing to lower satisfaction.

#### **Department Referrals**

Most patients (**5,400**) did not require referrals after their ER visit. Among referred patients, **General Practice** and **Orthopedics** accounted for the highest referral volumes, highlighting these departments as key areas supporting emergency care.

#### **Peak Demand**

Patient visits were highest on **Mondays, Saturdays, and Tuesdays**, with peak attendance occurring around **11 AM, 1 PM, 7 PM,** and **11 PM**. These periods may require increased staffing and resource allocation to maintain service efficiency.

#### **Patient Demographics**

Adults aged **20–39 years** represented the largest patient group, while **White** and **African American** patients accounted for the largest racial demographics. Admissions were evenly split between patients who were hospitalized and those discharged after treatment.