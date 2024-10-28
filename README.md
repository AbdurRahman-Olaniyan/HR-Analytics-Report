# HR Analytics Report

This project demonstrates my skills in designing and developing comprehensive analytics reports and dashboards using Microsoft Excel. Created as part of my mentorship program at [Analytics Extra](https://www.linkedin.com/company/analytics-extra/), it focuses on HR data analysis, offering insights into workforce demographics, turnover, satisfaction, and salary trends through advanced Excel features, including Power Pivot and DAX measures.

---

## Overview

In HR, data-driven insights are essential for decision-making. This project addresses key questions about employee demographics, turnover, satisfaction, and salary trends by developing interactive dashboards and analytics reports. Using Microsoft Excel’s Power Pivot and DAX capabilities, I created a dynamic report to support workforce planning, retention strategies, and HR performance analysis.

---

## Key Questions Addressed

This project answers the following key questions:

1. **What is the total number of employees since inception?**
2. **What is the total number of current employees?**
3. **What is the total number of terminated employees?**
4. **What is our employee termination rate?**
5. **What is the total salary paid to date?**
6. **What is the current employee distribution by gender?**
7. **What are the education levels of our employees?**
8. **How satisfied are our employees with their job?**
9. **What is the rate of our employees’ work-life balance?**
10. **What are our quarterly new hires?**
11. **What are our quarterly terminations?**
12. **What are the monthly termination trends?**
13. **What are the monthly salary trends?**
14. **What is the salary distribution by tenure for full-time employees and contractors?**
15. **What is the salary distribution by total working years of employees by gender?**

---

## Dataset Fields

![Dataset](https://github.com/user-attachments/assets/0bc5973f-38a6-4ca3-a2c8-5ee38e3f0f6c)

The dataset used for this analysis includes the following fields:

- **ID_employee**: Unique identifier for each employee
- **Age**: Age of the employee
- **Attrition**: Indicates if the employee has left the company
- **BusinessTravel**: Frequency of business travel
- **Department**: Department of employment
- **Education**: Education level
- **EnvironmentSatisfaction**: Satisfaction with work environment
- **Gender**: Gender of the employee
- **JobInvolvement**: Level of job involvement
- **Job Role**: Job role/title
- **JobSatisfaction**: Satisfaction with job role
- **PerformanceRating**: Performance rating
- **WorkLifeBalance**: Work-life balance rating
- **MaritalStatus**: Marital status of the employee
- **StockOption**: Stock option level
- **OverTime**: Whether the employee works overtime
- **PercentSalaryHike**: Percentage increase in salary
- **NumCompaniesWorked**: Number of companies previously worked at
- **TotalWorkingYears**: Total working years in career
- **YearsSinceLastPromotion**: Years since the last promotion
- **YearsWithCurrManager**: Years with the current manager
- **DistanceFromHome**: Distance from home to work (in miles)
- **HourlyRate**: Hourly wage rate
- **DailyRate**: Daily wage rate
- **MonthlyRate**: Monthly wage rate
- **Salary**: Current salary
- **TrainingTimesLastYear**: Number of training sessions attended in the last year
- **DateToday**: Current date for reference
- **DateBirth**: Employee’s birth date
- **DateStart**: Date of starting employment
- **DateDeparture**: Departure date (if applicable)
- **YearsAtCompany**: Total years spent at the company
- **AgeGroup**: Age group category
- **TerminationType**: Type of employment termination (if applicable)
- **AgeHire**: Age when hired
- **HireType**: Type of hire (e.g., direct, contract)
- **YearsAtCompany Group**: Grouped years of tenure at the company
- **EmploymentType**: Employment type (e.g., full-time, part-time, contractor)

---

## Key Metrics and DAX Measures

This project uses various metrics and DAX measures to provide actionable insights into employee demographics, salary trends, and turnover rates. Key measures include:

| **Metric**             | **DAX Measure**                                                                                   |
|------------------------|--------------------------------------------------------------------------------------------------|
| **Total Employees**    | `=COUNT(Employee[ID_employe])`                                                                   |
| **Headcount**          | `=CALCULATE([Total Employee], Employee[Attrition]="No")`                                         |
| **Terminations**       | `=CALCULATE([Total Employee], Employee[Attrition]="Yes")`                                        |
| **Termination Rate**   | `=[Termination] / [Headcount]`                                                                   |
| **Total Salary Paid**  | `=CALCULATE(SUM(Employee[Salary]), Employee[Attrition]="No")`                                    |

---

## Power Pivot Tables

![PivotTable](https://github.com/user-attachments/assets/5ee48bc0-9f94-4567-b65f-cf05441e4c85)

The following Power Pivot tables helped answer the key questions listed above by providing essential insights into employee demographics, satisfaction, and turnover trends.

1. **Employee Metrics**: This table includes `Total Employee`, `Headcount`, `Termination`, `Termination Rate`, and `Total Salary`, which are essential for understanding overall workforce composition and turnover rates.
2. **Gender Breakdown**: Displays employee `Headcount` by `Gender`, helping answer questions about gender distribution in the current workforce.
3. **Education Levels**: Shows `Headcount` by employee `Education`, useful for assessing the educational background across the organization.
4. **Job Satisfaction**: Displays `Headcount` by `JobSatisfaction` levels, providing insight into employee satisfaction.
5. **Work-Life Balance**: Tracks `Headcount` by `WorkLifeBalance`, giving an overview of work-life balance among employees.
6. **Quarterly New Hires and Terminations**: This table monitors `New Hires` and `Terminations` by `DateStart` (Quarter), helping visualize quarterly workforce changes.
7. **Monthly Terminations**: Monitors `Terminations` by `DateStart` (Month) to identify monthly termination trends.
8. **Monthly Salary Trends**: Tracks `Total Salary` by `DateStart` (Month), allowing a view of salary distributions over time.
9. **Salary by Tenure (Years at Company)**: Compares `Contractor` status with tenure, displaying `Grand Total`, which answers questions about salary by length of employment.
10. **Salary by Experience (Total Working Years)**: Breaks down `Total Salary` by `TotalWorkingYears`, `Gender`, and displays `Grand Total`, providing insight into experience-based salary distribution.

---

## Configuration and Setup

1. **Excel Version**: Make sure you are using a version of Microsoft Excel that supports Power Query and Power Pivot to utilize DAX and data modeling features.
2. **Data Structure**: Organize the dataset with columns matching the fields listed above to ensure correct calculations and visualizations.
3. **DAX Measures**: Input the DAX measures provided in the Power Pivot Measure Table to calculate key metrics for the dashboard.

---

## Key Highlights

- **Employee Metrics**: Track employee headcount, termination rate, and demographic distributions, with visuals that highlight trends and areas of interest.
- **Salary Analysis**: Review salary trends and distributions based on tenure and gender, helping to identify patterns in employee compensation.
- **Employee Satisfaction & Work-Life Balance**: Assess job satisfaction and work-life balance levels across different employee groups, supporting informed HR initiatives.
- **Hiring and Termination Trends**: Monitor monthly and quarterly trends in new hires and terminations to understand seasonal patterns in workforce changes.

---

## Insights Gained

![HR Dashboard](https://github.com/user-attachments/assets/e3efb3ee-59d5-4db5-ae9a-ae94fffaa751)

This analysis reveals key HR metrics, showing a total employee count of 1,470, with a current headcount of 1,233, where female employees constitute 40.6% and male employees 59.4%. A significant 38% of the workforce holds bachelor's degrees. The termination rate stands at 19.22%, indicating fluctuations in monthly trends that highlight the need for improved retention strategies. Moreover, over 60% of employees report a better work-life balance, with 30% expressing high job satisfaction. Salary trends indicate a correlation between tenure and compensation, providing valuable insights for data-driven HR decision-making aligned with organizational goals.
---
