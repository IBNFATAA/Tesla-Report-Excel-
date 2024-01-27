# Tesla Inventory Optimization Analysis


## Introduction
This is an excel project on car sales analysis of one of the renowned known company all over the wortld called **Tesla**.
The project is to analyze and derive insights to answer crucial questions, to know the trend and pattern of quantities ordered delivered and used in other to help the company make data driven decision.
decisions.
**_Disclaimer_** : This is an open real-life dataset of Tesla inventory scenario optimization.

## Problem Statement
1. summarize Total Quantities Ordered, Delivered and used with pivot tables 
2. Utilize conditional formatting to visually identify components with low inventory levels or those exceeding a specific threshold.
3. Implement a vlookup or index match function to cross-reference part numbers between different datasets and ensure accurate data consolidation.
4. Develop a dynamic charts that illustrates a trend in inventory levels overtime for a specific components.
5. Apply data validation to prevent errors in entering quantities or part numbers.

## Skills / Concepts Demonstrated
- Pivot Table
- Index and Match
- Conditional Formatting
- Data Validation
- Dynamic Table Creation
- Format Shape

## Problem Solved
1. In the "Past Orders" sheet, I select therange of data, including headers. Then I go to the "Insert" tab and click on "PivotTable."
Then place the PivotTable in a new worksheet. I drag "Sku ID" to the Rows area and drag "Order Quantity" to the Values area, and set it to show the sum of quantities. In the value field setting found in the Pivot table pane, I change the title to "Total Order Quantity". I repeated the process for the "Stock" sheet to summarize the 
"Total Delivered Quantity"(This was solved by creating a new column and using index and match to extract the quantities from Ordered Quantities) and "Used Quantity"(This was solved by subtracting Total Delivered Quantity from the current stock quantity). 

2. I choose the column with "Current Stock Quantity" in the "Stock" sheet.
go to Conditional Formatting:
go to the "Home" tab.
click on "Conditional Formatting" and choose "New Rule."
Set Conditions:Choose "Format cells that contain."
Set conditions like "Cell Value" less than to 219 (This 219 is as a result of average imputation of median used in Current Stock Quantity column.
Format with a color of red to visually identify low inventory.
Repeated for Exceeding Threshold: Added another rule for values exceeding a specific threshold (equal or greater than 219) using a different formatting color of green.

3. Apart from the fact that we use Index and Match it to create the column of "Total Delivered Quantity" it is also used to extract current stock quantity into "Past Order Sheet" from the "Stock Sheet" to cross-reference part numbers between different datasets and ensure accurate data consolidation..

### Conditional Formatting
## Visualization:
The Charts comprises 3 Line-Chart:
1. Current Stock Line Chart
2. Ordered Quantity Line Chart
3. Current Stock and Ordered Quantity Line Chart 

###  Current Stock Line Chart
In this Power BI sales analysis, I skillfully crafted a dynamic and comprehensive model. I implemented advanced measures, creating slicers for both month and segments to ensure seamless interaction with the report, line chart illustrate the sum of sales over months and years, allowing users to grasp sales trends without interference from slicers. Additionally, a doughnut chart visualizes sales distribution by ship mode. To highlight key categories, a stacked bar chart showcases the top 5 and bottom 5 sales, contributing to a comprehensive and interactive exploration of sales insights. The report seamlessly combines interactivity with user-friendly design, enabling stakeholders to make informed decisions and strategize effectively based on the presented data.



###  Ordered Quantity Line Chart
This Power BI report provides a detailed analysis of profit data with dynamic features such as buttons and slicers for month and segment selection. The primary focus is on a line chart illustrating the sum of sales over months and years, allowing users to grasp profits trends without interference from slicers. Additionally, a doughnut chart visualizes profit distribution by ship mode. To highlight key categories, a stacked bar chart showcases the top 5 and bottom 5 sales, contributing to a comprehensive and interactive exploration of tremendous insights when it comes to profit. The report seamlessly combines interactivity with user-friendly design, enabling stakeholders to make informed decisions and strategize effectively based on the presented data.



### Current Stock and Ordered Quantity Line Chart 



### Whole Report

## Conclusion and Recommendation
The insights generated from the report shows:
- The highest generated sales by Month and year = (NOVEMBER)
- Highest sales by ship mode = (STANDARD CLASS)
- Highest sales by CITY = (NEW YORK)
- Worst sales by city = (Waco)
- The highest generated profit by Month and year = (OCTOBER)
- Highest profit by profit = (STANDARD CLASS)
- Highest profit by profit = (NEW YORK)
- Worst sales by profit = (ELYRIA)
