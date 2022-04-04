# Pewlett Hackard

**Overview**
The purpose of this challenge was to determine which employees at Pewlett Hackard, a large corporation, will be retiring in the coming years, and therefore how many new employees must be hired.  Employees who were born between the years 1952 and 1955 and hired between 1985 and 1988 are "soon to be retirees".  In addition, Pewlett Hackard plans to designate employees born in the year 1965 as mentors for new hires.  A second database analysis was conducted to determine which employees are eligible to serve as mentors.

**Results**
For deliverable 1, the total number of retirees was calculated using the following code:
![image](https://user-images.githubusercontent.com/99574730/161474035-b9cdef21-80d6-4822-8aad-f7c7b9703ca1.png)
![image](https://user-images.githubusercontent.com/99574730/161474067-247fc306-9884-4e32-bcc1-70a819223fb2.png)

The above query initially determined the number of employees born between 1952 and 1955 - however, it failed to take into account the employees who had been promoted.  Therefore, although all the employees born from 1952-1955 were compiled, many were duplicates.  In order to gain a more accurate understanding, the Unique Titles table was created (this time without duplicates).  From this table, it was determined that 90,398 employees are retiring soon.

![image](https://user-images.githubusercontent.com/99574730/161475064-8c62f5fa-2049-4ee5-9fa2-7f5216e20172.png)

For deliverable 2, the number of Pewlett Hackard employees born in 1965 and eligible for mentorship was determined.  To train the 90,000+ new hires, Pewlett Hackard wants to implement a mentorship program in which senior employees will train newer hires.  The following query was written:

![image](https://user-images.githubusercontent.com/99574730/161475252-35a9d284-2bbd-4cd0-ba32-f65c8dea91d0.png)

This tabulated Pewlett Hackard employees born in the year 1965 (pulled from the existing dept_emp CSV file).  Overall, 1549 employees can serve as mentors.

**Summary**
Overall, 90,398 employees out of 300,024 employees are eligible for retirement (or roughly 30.13% of the current Pewlett Hackard workforce):

![image](https://user-images.githubusercontent.com/99574730/161471190-7c75b660-d60c-4562-b870-4f050bd7adaa.png)

Approximately 50% of the 90,398 employees making up the "silver tsunami" are engineers.  In total, 45,397 open senior engineer, assistant engineer, and engineer positions will need to be filled.

However, only 1549 Pewlett Hackard employees are currently eligible to serve as mentors for new hires:
![image](https://user-images.githubusercontent.com/99574730/161471425-1544e30d-a385-4bce-85ce-1994e5cb7dde.png)

Since the company will hire 90,398 new employees, each mentor would need to mentor ~58 junior employees.  This will likely be very difficult, and more mentors will be needed.  Expanding the mentorship eligibility criteria to include employees born between 1964 and 1967, for example, may mitigate the issue.
