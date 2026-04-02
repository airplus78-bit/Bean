# Apply filters to SQL queries

## Project description

\[My task is to examine the organization’s data in their **employees** and **log\_in\_attempts** tables. I use SQL filters to retrieve records from different datasets and investigate the potential security issues.I recently discovered a potential security incident that occurred after business hours.A suspicious event occurred on 2022-05-09. There’s been suspicious activity with login attempts, but the team has determined that this activity didn't originate in Mexico. I investigated login attempts that occurred outside of Mexico\]

## Retrieve after hours failed login attempts

SELECT \*  
FROM log\_in\_attempts  
WHERE login\_time \> ‘18:00’ AND SUCCESS \= FALSE;\]

## Retrieve login attempts on specific dates

\[ SELECT \*  
FROM log\_in\_attempts   
WHERE login\_date \= ‘2022-05-09’ and ‘2022-05-08’;.\]

## Retrieve login attempts outside of Mexico

\[SELECT \*  
FROM log\_in\_attempts  
WHERE NOT country \= ‘MEX%’;.\]

## Retrieve employees in Marketing

SELECT \*  
FROM employees  
SELECT department \= ‘Marketing’

## Retrieve employees in Finance or Sales

\[SELECT \*  
FROM employees  
WHERE department \= ‘Finance’ OR department \= ‘Sales’;Add content here.\]

## Retrieve all employees not in IT

\[SElECT \*  
FROM employees  
WHERE NOT department \=’Information Technology’;Add content here.\]

## Summary

organization database contains the following two tables:  
● log\_in\_attempts  
● employees

log\_in\_attempts  
The log\_in\_attempts table has the following columns:  
● event\_id: The identification number assigned to each login event  
● username: The username of the employee  
● login\_date: The date the login attempt was recorded  
● login\_time: The time the login attempt was recorded  
● country: The country where the login attempt occurred  
● ip\_address: The IP address of that employee’s machine  
● success: The success of the login attempt; FALSE indicates a failed attempt  
\[

● employee\_id: The identification number assigned to each employee  
● device\_id: The identification number assigned to each device used by the employee  
● username: The username of the employee  
● department: The department the employee is in  
● office: The office the employee is located in  
Add content here.\]  
