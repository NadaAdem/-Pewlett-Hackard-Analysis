# Pewlett Hackard Analysis

## Overview of Project

The purpose of this project is to analyze the employment database of  'Pewlett-Hackard' to find the number of retiring employees by position. To prepare for the incoming waves of retirement, it is suggested to create a mentorship program to train the  employees for new postions . 



## Resources and Software

The following six CSV data files were provided at the beginning of the analysis:
- departments.csv, employees.csv, salaries.csv, dept_emp.csv, dept_manager.csv, titles.csv are found inside of the Data folder.
- PostgreSQL 13.2
- pgAdmin 4.50



## Results
The table below shows the number of retirement age employees born between January 1, 1952 and December 31, 1955 grouped by title in the company.

 ![This is an image](https://github.com/NadaAdem/-Pewlett-Hackard-Analysis/blob/main/Resources/retiring_titles.png)

- The positions most affected by the incoming wave of retirement will be "Senior Engineer" and "Senior Staff."
- A total of 90,398 employees are retiring or nearing retirement.
- Two managers are retiring, which is significant because there are only nine current managers.
- 1,549 current employees born between January 1, 1965 and December 31, 1965 are eligible to participate in the mentorship program.

## Summary
There will need to be 90,398 roles filled across all departments.Pewlett-Hackard will need to train new employees to fill these vacant positions.Beside, two high-level managment positions must be filled.

- The query to create this mentorship table is:
SELECT COUNT(emp_no), title
FROM mentorship_eligibility
GROUP BY title
ORDER BY count DESC;

 ![This is an image](https://github.com/NadaAdem/-Pewlett-Hackard-Analysis/blob/main/Resources/mentorship_eligibility_COUNT.png)
 
 
After analyzing ,1,549 current employees would qualify for becoming mentors. for perpare incoming wave of retirement facing Pewlett-Hackard is  increasing the number of both mentors and new employees.
