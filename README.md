# HR Analytics Dashboard – Employee Attrition Analysis

End-to-end HR analytics project focused on understanding and predicting employee attrition.

- **Data cleaning** → Excel  
- **Database & analysis** → Oracle SQL + PL/SQL  
- **Visualization & interactivity** → Power BI

## Problem Statement
- Identify the key factors contributing to employee attrition.
- Analyze attrition trends across departments, job roles, and salary levels.
- Examine how experience, age group, and demographics impact turnover.
- Measure overall attrition rate and identify high-risk employee segments.

## Technologies Stack

- Oracle Database (SQL & PL/SQL)  
- Microsoft Excel (data cleaning)  
- Microsoft Power BI (interactive dashboard)  
- Dataset: IBM HR Employee Attrition & Performance (classic dataset)

## Key SQL Queries (20)

| #  | Topic                                      | Technique used                     |
|----|--------------------------------------------|-------------------------------------|
| 1  | Employees per Department                   | GROUP BY                            |
| 2  | Avg Salary per Department                  | ROUND(AVG())                        |
| 3  | Attrition count & % per Department         | CASE + conditional aggregation      |
| 4  | Employees above dept average salary        | Correlated subquery                 |
| 5  | Top 5 highest paid employees               | ORDER BY + ROWNUM                   |
| 6  | >5 years exp + Overtime = Yes              | Simple WHERE                        |
| 7  | Gender distribution by Department          | GROUP BY multiple columns           |
| 8  | Avg salary by JobRole (HAVING >5000)       | HAVING clause                       |
| 9  | Employees never promoted                   | YearsSinceLastPromotion = 0         |
| 10 | Salary rank inside each department         | Correlated COUNT(DISTINCT)          |
| 11 | Second highest salary company-wide         | Subquery                            |
| 12 | Employees worked in >3 companies           | Simple filter                       |
| 13 | Age group buckets & count                  | CASE WHEN                           |
| 14 | Department with highest avg salary         | ORDER BY + ROWNUM                   |
| 15 | Highest paid employee per department       | Correlated MAX()                    |
| 16 | Overtime Yes vs No count                   | GROUP BY                            |
| 17 | Employees with above-average Performance   | Subquery                            |
| 18 | TotalWorkingYears > YearsWithCurrManager   | Comparison                          |
| 19 | % distribution by EducationField           | COUNT / total subquery              |
| 20 | Running total salary per department        | SUM() OVER (PARTITION BY … ORDER BY)|

## PL/SQL Components

```sql
-- Procedure: overall attrition summary
EXEC Calculate_Attrition_Rate;

-- Function: attrition count by department
SELECT Get_Department_Attrition('Sales') FROM DUAL;
SELECT Get_Department_Attrition('Research & Development') FROM DUAL;
