
# Pewlett Hackard Challenge

## Overview of the analysis
As the 300,024 employees of the Pewlett Hackard company age, there is the concern that a large number of employees will be retiring soon.  To prepare for this "silver tsunami", it is prudent to discover the number of employees that may be eligible for retirement as well as the number of employees that may be eligible for a mentorship program. 

1. Created a Retiring Titles table that shows the number of retirement eligible employees by job title. 
2. Created a Mentorship Eligibilty table that shows the number of mentorship eligible employees.  For these purposes we will assume that employees born in the year 1965 are mentorship eligible.
3. Created tables that show the number of retirement eligible employees and mentorship eligible employees by department.

## Resources
- Data Source: departments.csv, dept_emp.csv, dept_manager.csv, employees.csv, salaries.csv, titles.csv
- Software: pgAdmin 4

## Results
* The number of retirement eligible employees (employees born between 1952 and 1955) is very large.
	*  By far the largest number of retirement eligible employees are the Senior Engineers and the Senior Staff with 25,916 and 24,926 eligible respectively.
	* The total number of retirement eligible employees is 72,458.
	
![Retiring Titles](https://github.com/BlazeMedina/Pewlett-Hackard-Analysis/blob/main/queries/retiring_titles.png)

* Maintaining the requirement that mentorship eligible employees must have been born in 1965, the number of mentorship employees is comparatively small, 1,549.

![Mentorship Eligibility](https://github.com/BlazeMedina/Pewlett-Hackard-Analysis/blob/main/queries/mentorship_eligibility.png)
## Summary
The number of retirement eligible employees is nearly 25% of the current workforce.  The mentorship program should not be confined to only accept applicants born in 1965 but should instead take into account how long they have been employed at Pewlett Hackard and how long they have held their current title.  Assuming that Pewlett Hackard would like to replace the employees that may retire, an agressive hiring model should be executed to replace the 72,458 that may retire.  Further analysis shows that the largest number of retirement eligible employees are from the departments; Development, Production, and Sales.

![Department Retiring](https://github.com/BlazeMedina/Pewlett-Hackard-Analysis/blob/main/queries/dept_retiring.png)

Assuming the mentorship eligibility requirements remain the same, there will be a sufficient number of retirement-ready employees in each department to mentor the next generation Pewlett Hackard employee.

![Department Retiring vs Department Mentorship Eligible](https://github.com/BlazeMedina/Pewlett-Hackard-Analysis/blob/main/queries/dept_ret_vs_ment.png)
