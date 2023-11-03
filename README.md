# World-Bank-Debt
The World Bank's external debt data is a valuable resource for data analysts, economists, policymakers, and researchers. It provides insights into the financial health and economic relationships of countries across the world. This visualization focuses on the countries with the highest debt, using PowerBI. Here are some steps that went into getting insight:
-- I had questions in mind and a problem I wanted to solve included knowing: i) the total amount of debt that is owed by the countries listed in the dataset; ii) Country with the maximum amount of debt; and iii) The bottom 5 countries iv) YoY

-- Now that I knew what problem I wanted to solve, I downloaded the dataset from worldbank.org
-- Did a little cleaning of the footer that automatically got downloaded with the data
-- Import data to PowerBI using get data
-- Transformed the data in Power Query Editor so it is readable by
i) Promoting the headers using the first row
ii) Removed empty columns, mainly years with no record
iii) Selected the necessary columns and unpivot the rest of the columns, which reduced about 15 columns to 2
iv) Renamed columns for better understanding
v) The year column had repeated values separated by [], I split column by that delimeter and replaced with none
vi) Removed the duplicated year column
vii) The data only had a year column, then I got the date column by adding a custom column with 04-01 with the numbers.totext function
viii) Now that the data is cleaned and readable, went on to close and apply.

-- It was compulsory to create measures such as DistinctCount to get distinct total country numbers, SUM, and calendar auto to get a calendar table.

