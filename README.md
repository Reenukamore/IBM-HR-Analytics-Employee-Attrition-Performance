**Project Title**  
IBM HR Analytics Employee Attrition & Performance

**Domain**  
Human Resources Analytics | Data Analysis

**Difficulty Level**  
Intermediate

**Tools Used**  
- Excel (Data Cleaning & Initial Exploration)  
- SQL Developer (Oracle) – Advanced querying & aggregations  
- Power BI – Interactive Dashboard & Visualizations

**Dataset**  
Fictional HR dataset created by IBM data scientists. 
Contains 1,470 employee records with 35 features including age, job role, monthly income, job satisfaction, work-life balance, distance from home, overtime, etc.

## Business Problem

Companies face high employee turnover (attrition), which increases recruitment & training costs, disrupts team dynamics, and causes loss of valuable knowledge.  
This project uncovers **why employees leave** and helps suggest retention strategies.

## Objectives

1. Calculate current **attrition rate** and analyze distribution by demographics (age, gender, department, job role, education, etc.).  
2. Identify **key drivers** of attrition:  
   - Job satisfaction (JobSatisfaction, EnvironmentSatisfaction, RelationshipSatisfaction)  
   - Work-life balance & job involvement  
   - Salary & benefits (MonthlyIncome, PercentSalaryHike, StockOptionLevel)  
   - Other factors: OverTime, DistanceFromHome, YearsAtCompany, etc.  
3. Build an **interactive Power BI dashboard** to explore insights visually.

## Project Workflow

1. **Data Cleaning** – Excel  
   - Removed duplicates (none found)  
   - Checked & handled missing values (none)  
   - Validated data types & ranges  

2. **Data Analysis with SQL** – Oracle SQL Developer  
   - Calculated attrition rate  
   - Aggregations: avg income by education/attrition, count by job role/department, etc.  
   - Breakdowns: distance from home by job role & attrition  

3. **Visualization & Dashboard** – Power BI  
   - Interactive dashboard with slicers (department, job role, gender, etc.)  
   - Key visuals: attrition rate card, age distribution, income vs education, factors comparison  

## Key Findings (Sample Insights)

- Overall **attrition rate** ≈ **16.12%**  
- Employees who work **OverTime** have significantly higher attrition  
- Lower **JobSatisfaction**, **EnvironmentSatisfaction**, and **WorkLifeBalance** strongly correlate with leaving  
- Younger employees (20–30 age group) and those with **longer distance from home** show higher turnover  
- Single employees and certain job roles (e.g., Sales Representative, Laboratory Technician) have elevated risk


