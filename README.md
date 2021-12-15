# Pewlett-Hackard-Analysis
Performing employee research to help Pewlett Hackard HR Analyst, Bobby, identify individuals who will soon be retiring and how many positions will soon be open.

## Overview of the analysis:
In this analysis, we helped perform data analysis for Pewlett Hackard, a company with an aging population who will soon be retiring and leaving many positions open. 

The company currently only houses information in CSVs, so we first created a database and tables to house the information from the CSVs. We then were able to query the data to determine the following:
- Who was eligible to retire
- Determine how many current employees exist by department
- Create a list of employee information
- Create a list of management information
- Create a list of retirees by department

We then determined the following:
1) The Number of Retiring Employees by Title
2) The Employees Eligible for the Mentorship Program

## Results:

- Based on the below (retirement_titles), we can see all employees and employee information, including employee number, first name, last name, and what title(s) they have or had. This table shows us that certain employees have had numerous different titles over the course of their employement with Pewlett Hackard.

<img width="495" alt="image" src="https://user-images.githubusercontent.com/92613639/146120448-62c37a5b-100c-4888-bc2b-9aeb06e0c735.png">

- Based on the below (unique_titles), we are able to see only the most recent or current job title for each employee. This table as is shows a line per employee so this is useful if you want to look into a specific employee, but may not be super helpful for company-wide analysis.

<img width="364" alt="image" src="https://user-images.githubusercontent.com/92613639/146120932-d1fbe8ce-848b-4967-bb5d-cce48132c8b6.png">

- From the below, (retiring_titles), we are able to see the employee count by most recent or current job title for all employees. This can give us an idea of how employees are distributed among job titles. Based on the below, we can see that if a few 'Senior Engineers' were to retire, it may not be such a big deal, but if a couple 'Managers' retire, you would have no managers left.

<img width="151" alt="image" src="https://user-images.githubusercontent.com/92613639/146121448-5fa418b6-efbf-4db0-a7f5-e0a4615de822.png">

- The below query (mentorship_eligibility), shows us a list of all current employees who are eligible for the mentorship program based on an age criteria. This list can help you determine who can be promoted to fill some of the open positions resulting from the "Silver Tsunami."

<img width="553" alt="image" src="https://user-images.githubusercontent.com/92613639/146121738-d4865173-4669-4ac5-a5a1-0db4b41e0601.png">


## Summary:
Summary: Provide high-level responses to the following questions, then provide two additional queries or tables that may provide more insight into the upcoming "silver tsunami."
Q: How many roles will need to be filled as the "silver tsunami" begins to make an impact?
A: According to 'retiring_titles," there are 90,398 roles that will be opening up soon. However, when we add the'to_date' column to the unique_titles query, we can see that this number includes individuals who retired in the past (ex: Marry Sluis left the company in 1996). This means the actual number of individuals retiring now will be lower. It would be a good idea to add a query (1) that removes already retired/terminated employees and only includes the number of current employees who are up for retirement.

<img width="413" alt="image" src="https://user-images.githubusercontent.com/92613639/146125653-9d7e9938-32e8-448a-afb1-d01ca2ef6e2c.png">

By doing so, we get the following revised number (72,458 total) of current employees eligible for retirement - see below.

<img width="243" alt="image" src="https://user-images.githubusercontent.com/92613639/146126130-9db0e013-dffa-437f-8f8d-63fb0f7a47c9.png">

Q: Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?
A: 
