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

4. In other to develop a dynamic charts that illustrates a trend in inventory levels overtime for a specific components. I combined data.By
Creating a new sheet to combine relevant data from both the "Past Orders" and "Stock" sheets. Assuming you have columns like "Order Date," "Sku ID," "Order Quantity," and "Current Stock Quantity," arrange them in a structured manner which i already have in my Past orders sheet.
Created a Line Chart:Select Data Range:Highlight the range of data, including headers, that I want to include in my dynamic chart. I ensured it covers "Order Date," "Order Quantity," and "Current Stock Quantity."Inserted a Line Chart:Go to the "Insert" tab on the Excel ribbon.Clicked on "Line" under the "Charts" section.Adjust Chart Design:
I adjust the chart design, titles, and labels as needed for better clarity.
#### Visualization:
The Charts comprises 3 Line-Chart:
i. Current Stock Line Chart

ii. Ordered Quantity Line Chart

iii. Current Stock and Ordered Quantity Line Chart 

I Made Chart Dynamic By:
Converting Data to Excel Table 
Press Ctrl + T to convert the range into an Excel Table. 
Define dynamic named ranges for your data. This step is optional but can be helpful.
Go to the "Formulas" tab, click on "Name Manager," and created new named ranges using formulas that automatically adjust to new data in case we have new data.






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
