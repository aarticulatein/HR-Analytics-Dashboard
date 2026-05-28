# HR Analytics Dashboard – Employee Attrition & Retention Insights

##  Project Overview

This project focuses on analyzing employee attrition trends using the IBM HR Analytics Employee Attrition & Performance dataset.  
The dashboard was developed in Power BI to identify key factors influencing employee turnover and provide actionable workforce insights.

The analysis helps answer important business questions such as:

- Which employees are leaving the organization?
- What factors contribute to attrition?
- Which employee groups are at higher retention risk?
- How can HR teams improve employee retention strategies?

---

# Objectives

- Analyze employee attrition patterns
- Identify major attrition drivers
- Build interactive HR analytics dashboard
- Enable data-driven HR decision making
- Improve workforce retention analysis

---

# Tools & Technologies Used

- Microsoft Power BI
- Microsoft Excel
- Power Query
- DAX (Data Analysis Expressions)

---

# Dataset

Dataset Used:
IBM HR Analytics Employee Attrition & Performance Dataset (Kaggle)

Dataset includes:
- Employee demographics
- Salary information
- Department & job roles
- Work-life balance
- Job satisfaction
- Promotion history
- Overtime details
- Attrition status

---

# Data Cleaning & Transformation

Data preprocessing was performed using Power Query in Excel and Power BI.

Key transformations included:

- Handling null values
- Removing duplicates
- Creating Salary Slabs
- Creating Age Groups
- Creating Work-Life Balance Levels
- Creating Promotion Risk categories
- Creating Tenure Groups
- Formatting and standardizing columns

---

# Dashboard Features

## Executive KPIs
- Total Employees
- Average Salary
- Attrition Count
- Attrition Rate %
- Overtime %

## Attrition Analysis
- Attrition by Department
- Attrition by Salary Slab
- Attrition by Age Group
- Attrition by Gender
- Attrition by Job Satisfaction
- Attrition by Work-Life Balance
- Attrition by Promotion Risk
- Attrition by Tenure Group
- Attrition by Overtime

## Interactive Features
- Department Filters
- Job Role Filters
- Gender Filters
- Age Group Filters

---

# Key Business Insights

- Employees in the low salary slab showed the highest attrition.
- Employees working overtime contributed significantly to employee turnover.
- Low job satisfaction strongly correlated with higher attrition.
- New joiners exhibited higher attrition rates compared to experienced employees.
- Work-life balance and promotion-related factors influenced employee retention trends.

---

# Dashboard Preview

![Dashboard](screenshots/dashboard.png)

---

# Skills Demonstrated

- Data Cleaning
- Data Transformation
- Data Modeling
- DAX Calculations
- Data Visualization
- Business Intelligence
- HR Analytics
- Dashboard Design
- Analytical Storytelling

---

# DAX Measures Used

```DAX
Total Employees = COUNTROWS(HR_Analytics_Cleaned)

Attrition Count =
CALCULATE(
    COUNTROWS(HR_Analytics_Cleaned),
    HR_Analytics_Cleaned[Attrition] = "Yes"
)

Attrition Rate % =
DIVIDE(
    [Attrition Count],
    [Total Employees],
    0
)

Avg Salary =
AVERAGE(HR_Analytics_Cleaned[MonthlyIncome])

---

## Project Outcome

The dashboard provides actionable insights into employee attrition patterns and workforce retention trends.

---

## Author

Aarti Sharma

Aspiring Data Analyst skilled in Power BI, Excel, SQL, and HR Analytics.

