# Hewlitt-Packard_Analysis
## Problem
In this challenge the problem we needed to solve was to create tables from CSV files to create newer tables. These newer tables answered the questions in the challenge prompts. The crux of the problem was to gather data that would better prepare Hewlitt Packard for the wave of employees who were about to retire. Another problem was to figure out who was eligible for the mentorship program. 
## Steps to solve the problem
The first step to solving the problem was to create a table containing the number of employees who were about to retire. This table needed to include employee number, first name, last name, title, from date, and salary. To do this we used an inner join function. We used that function on the salries and titles tables we created in the module. Next we partitoned the data to remove repition. The next step was to create three new tables. The first table was to show the number of titles retiring. To do this I used a left join using the titles table and a group by function by the titles table. The second table was showing the number of people retiring which was 41,380. To achieve this I used a where function with specific dates that matched the data needed, 1952-01-01 and 1955-12-31. The third table was to find the number of employees by title. To achieve this I used a left join on titles, but used a from function from the employees table.  Next, I needed to make a table for mentorshi eligibility. To do this I first partitioned the data to eliminate any repition. Next I used a from statement for employees and inner joined recent title table and the titles table. There were many challenges when trying to get this data and code to work properly. First was deciding which tables to pull from and join together. I had to check each table to see what columns it contained. This helped me discover the view function in pgadmin, where you are able to view tables directly in the application rather than pulling up each and every CSV file seperatly and repeatedly. Another issue was aliases, these are simple in priciple, but the problem is just remembering to include them in the code and to do so accurately. 
## Results
In  this challenge we found many results. First, the number of those retiring was 41,380. Second the number of those eligible for the mentorship program which was 1549. We also found out that those retiring by title was as follows: Assistant Engineer-2037, Engineer- 16,111, Manager-5, Senior Engineer-15,600, Senior Staff-14,736, Staff-14924, Technique Leader-2,014. Next we found the employee count by title which was as follows: Assistant Engineer-15,128, Engineer- 115,003, Manager-24, Senior Engineer-97,750, Senior Staff-92,853, Staff-107,391, Technique Leader-15,159. A limitation I found was that there is no data or metric that calculates employees contributions. I know this is hard to quantify, but if we had that metric we could make some calculations on return on investment with those retiring as well as have another way of quantifying performance of current employees. Some next steps I would reccomend would be to find out how those retiring enjoyed working there, maybe take a survey and ask if they have any ideas to improve the work life for future employees. Those retiring would be the perfect people to ask this sort of question. 

![ERD](C:\Users\mattd\Documents\2020 Vandy Bootcamp\Module 7 Analysis Projects Folder\Pewlett-Hackard-Analysis Folder\ERD Pictures)
Format: ![Alt Text](url)
