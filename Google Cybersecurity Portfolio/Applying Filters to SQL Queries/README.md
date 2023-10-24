**TASK**


I work as a security professional in a prominent organization, and one of my key responsibilities involves investigating security concerns to maintain the integrity of our systems. Recently, I came across a set of potential security problems related to login attempts and the devices used by our employees.

My current assignment requires me to delve into the organization's data, specifically within the 'employees' and 'log_in_attempts' tables. To address these potential security issues, I'm tasked with employing SQL filters to extract and examine records from various datasets, ultimately aiming to identify and address these security concerns effectively.

I completed this task by doing the following:

1. **Retrive after hours failed login attempts**

I've just uncovered a potential security incident that took place outside of regular business hours. In order to get to the bottom of this, I'm required to interrogate the 'log_in_attempts' table and scrutinize login activities that occurred after the close of business. To do this, I'll be utilizing SQL filters to construct a query that pinpoints all unsuccessful login attempts that happened after 18:00. This information can be extracted from the 'login_time' column.

2. **Retrieve login attempts on specific dates**

On  2022-05-09, we observed an event that raised suspicions. To get to the bottom of this incident, I'm planning to examine all login attempts that took place on both 2022-05-09, and the day preceding it. To achieve this, I'll be making use of SQL filters to construct a query that singles out all login attempts recorded on either 2022-05-09, or 2022-05-08. This information can be extracted from the 'login_date' column.

3. **Retrieve login attempst outside of Mexico**

We've detected some concerning login activity, but our team has confirmed that this activity did not originate from Mexico. The next step is to dig deeper and scrutinize login attempts that occurred beyond the borders of Mexico. To accomplish this, I will be applying SQL filters to construct a query that isolates all login attempts originating from locations other than Mexico. It's worth noting that when referencing Mexico, the 'country' column includes values like MEX and MEXICO, so I'll use the LIKE keyword with '%' to ensure that our query accurately reflects this distinction.

4. **Retrieve employees in marketing**

My team has initiated a security update project targeting specific employee machines within the Marketing department. I have been assigned the task of collecting information about these particular employee machines, which entails querying the 'employees' table.
In order to accomplish this, I'll be using SQL filters to construct a query that narrows down the results to include only employees within the Marketing department and who work in offices located within the East building. To do this, I will use the LIKE keyword with '%' to filter for office values that fall under the East building. The 'department' column will help me identify employees in the Marketing department, and the 'office' column contains values like East-170, East-320, and North-434, which I will use for filtering.

5. **Retrieve employees in finance or sales**

My team has a new task at hand, which involves carrying out a distinct security update for the machines used by employees in the Sales and Finance departments. To facilitate this, I'll be utilizing SQL filters to construct a query that pinpoints all employees who are part of either the Sales or Finance departments. The 'department' column holds the relevant information I need for this filter, as it contains values like Sales and Finance that will help me identify the employees in question.

6. **Retrieve all employees not in IT**

Our team has one more task to complete concerning updates for employee machines. Employees who belong to the Information Technology (IT) department have already received this update. However, employees from all other departments are still pending this update. 
To isolate these employees efficiently, I will employ SQL filters to construct a query that identifies all employees who are not part of the IT department. The 'department' column contains the necessary information, including values like Information Technology, to assist in this filtration process.
