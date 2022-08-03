![image](https://github.com/Bryan-Corn/Pewlett-Hackard-Analysis/blob/main/Images/HR.png)
# Pewlett-Hackard-Analysis
Module 7 

## Overview

Pewlett-Packard needs an analysis on their employee data. Senior management knows they have a lot of people getting close to retirement and they know they need to do something to prepare and put the company in a good position for the future, after these employees leave and take all of their collective institutional knowledge with them. 

For this task, there are three deliverables:


### Deliverable 1: The Number of Retiring Employees by Title

Using the ERD you created in this module as a reference and your knowledge of SQL queries, create a Retirement Titles table that holds all the titles of employees who were born between January 1, 1952 and December 31, 1955. Because some employees may have multiple titles in the database—for example, due to promotions—you’ll need to use the DISTINCT ON statement to create a table that contains the most recent title of each employee. Then, use the COUNT() function to create a table that has the number of retirement-age employees by most recent job title. Finally, because we want to include only current employees in our analysis, be sure to exclude those employees who have already left the company.


### Deliverable 2: The Employees Eligible for the Mentorship Program

Using the ERD you created in this module as a reference and your knowledge of SQL queries, create a mentorship-eligibility table that holds the current employees who were born between January 1, 1965 and December 31, 1965.


### Deliverable 3: A written report on the employee database analysis

For this part of the Challenge, you’ll write a report to help the manager prepare for the upcoming "silver tsunami."
The analysis should contain the following:

  • Overview of the analysis: Explain the purpose of this analysis.


  • Results: Provide a bulleted list with four major points from the two analysis deliverables. Use images as support where needed.


  • Summary: Provide high-level responses to the following questions, then provide two additional queries or tables that may provide more insight into the upcoming "silver tsunami."

     • How many roles will need to be filled as the "silver tsunami" begins to make an impact?
     • Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?

## Results

A relational database was created using the following ERD to determine the number of employees that will be retiring in the near future:

![image](https://github.com/Bryan-Corn/Pewlett-Hackard-Analysis/blob/main/Images/EmployeeDB.png)

Running the queries included the attached folder, the retiring, current, employees were identified and the total count of retirees with each current title was compiled into the following table with:

![image](https://github.com/Bryan-Corn/Pewlett-Hackard-Analysis/blob/main/Images/retiring_titles.png)


Filtering the table above to only those employees born in 1965 gives us a list of people nearing retirement that still have enough time left to share their knowledge and use their experience to pass the torch to the next generation of senior employees:
![image](https://github.com/Bryan-Corn/Pewlett-Hackard-Analysis/blob/main/Images/mentorship_eligibilty.png)


Please not that duplicates were removed from the table containing all retiring employees as individuals are listed with each title they have obtained during their tenure:

![image](https://github.com/Bryan-Corn/Pewlett-Hackard-Analysis/blob/main/Images/retiring_dups.png)


An additional table was added to show the percentage of each retiring title count:

![image](https://github.com/Bryan-Corn/Pewlett-Hackard-Analysis/blob/main/Images/retiring_titles_percent.png)


From these tables, we can glean the following:
```
• A total of 90,389 employees are ready for retirement and will need to be replaced
• 57668 of these retirees are in Senior Staff or Senior Engineer positions
• 70% of the 1550 employees eligible for mentorship are in these senior positions
• There are no managers on the list for mentorship eligibility
• The criteria for mentorship eligibility should be expanded to meet the demand to prepare the next generation to replace the upcoming retirement wave
```
