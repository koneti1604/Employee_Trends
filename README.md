# Employee Trends Analysis SQL Script

This repository contains an SQL script designed to analyze employee trends such as attrition rates, job satisfaction, and departmental statistics. The dataset is assumed to represent employee information from a fictional company.

---

## Features of the Script

### 1. **Employee Count by Department**
   - Counts the number of employees in each department.

### 2. **Average Age by Department**
   - Calculates the average age of employees for each department.

### 3. **Common Job Roles by Department**
   - Identifies the most common job roles in each department.

### 4. **Average Job Satisfaction by Education Level**
   - Analyzes job satisfaction scores based on education levels.

### 5. **Attrition Rate Analysis**
   - Calculates attrition rates for various age bands and education levels.

### 6. **Job Satisfaction Insights**
   - Determines age bands and education levels with the highest average job satisfaction.

---

## How to Use the Script

1. Ensure you have a database named `Employeet` with the appropriate table and data loaded.
2. Execute the SQL script in a tool like:
   - Microsoft SQL Server Management Studio (SSMS)
   - Azure Data Studio
3. Review the output of each query to gain insights into employee trends.

---

## Prerequisites

- **Database**: Ensure the `Employeet` database is set up.
- **Table Structure**: Ensure the employee table includes the following columns:
  - `department`
  - `age`
  - `job_role`
  - `job_satisfaction`
  - `attrition`
  - `education`
  - `business_travel`
  - `marital_status`
  - `age_band`

---

## Example Queries

- Employee Count by Department:
  ```sql
  SELECT department, COUNT(*) AS employee_count
  FROM Employeet
  GROUP BY department;
