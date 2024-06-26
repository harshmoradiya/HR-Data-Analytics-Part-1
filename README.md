HR DATA ANALYTICS PART-1

Project Overview
This project focuses on analyzing employee data to understand various aspects of workforce management. In Part 1, we model key performance indicators (KPIs) such as employee count and attrition rates. We then create calculated fields to derive meaningful insights and visualize the data using Tableau. The steps below outline the process in detail.

Key Performance Indicators (KPIs)
1. Employee Count
The total number of employees in the dataset.

2. Attrition
Attrition refers to employees leaving the company. We will calculate attrition count and attrition rate.

Calculated Fields
Attrition Count
To calculate attrition count, create a calculated field with the following formula:
sql
IF [Attrition] = 'Yes' THEN 1 ELSE 0 END


Attrition Rate
To calculate the attrition rate, use the formula:
sql
SUM([Attrition Count]) / SUM([Employee Count])


Active Employees
Calculate active employees using the formula:
sql
SUM([Employee Count]) - SUM([Attrition Count])
Visualizations
Attrition by Gender
This visualization shows the number of employees leaving the company categorized by gender.

Rows: Gender
Columns: SUM([Attrition Count])
Additional: Drag SUM([Attrition Count]) to the marks card, then right-click and select "Dual Axis."


Creating the Dashboard
In Tableau, combine the visualizations created above to form a comprehensive dashboard. This dashboard provides insights into employee attrition and other key metrics.
Next Steps
In Part 2, we will continue analyzing the data and refining our insights. Stay connected for the next update. Good luck!

Additional Resources
Data Source: HR dataset in Excel format
Screenshots: Included in the repository
r the next update. Good luck!

Additional Resources

Data Source: HR dataset in Excel format
Screenshots: Included in the repository
