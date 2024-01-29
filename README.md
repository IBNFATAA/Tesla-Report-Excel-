# Tesla Inventory Optimization Analysis

![Tesla_Made_Car](https://github.com/habeebsalaudeen/Tesla-Report-Excel-/assets/97491265/2381706e-2195-4928-bb7b-3b119f032462) | ![tesla_car](https://github.com/habeebsalaudeen/Tesla-Report-Excel-/assets/97491265/b1d1f81a-9e32-4691-95e3-5b15c888bed2)


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
1. In the "Past Orders" sheet, I selected the range of data, including headers. Then I go to the "Insert" tab and click on "PivotTable."
Then place the PivotTable in a new worksheet. I drag "Sku ID" to the Rows area and drag "Order Quantity" to the Values area, and set it to show the sum of quantities. In the value field setting found in the Pivot table pane, I changed the title to "Total Order Quantity". I repeated the process for the "Stock" sheet to summarize the 
"Total Delivered Quantity"(This was solved by creating a new column in the stock sheet and using index and match to extract the quantities from Ordered Quantities in the past orders sheet) and "Used Quantity"(This was solved by subtracting Total Delivered Quantity from the current stock quantity). 

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
Creating a new sheet to combine relevant data from both the "Past Orders" and "Stock" sheets. Having columns like "Order Date," "Sku ID," "Order Quantity," and "Current Stock Quantity," arrange them in a structured manner which i already have in my Past orders sheet.

Afterwards, I created a Line Chart:Select Data Range:Highlight the range of data, including headers, that I want to include in my dynamic chart. I ensured it covers "Order Date," "Order Quantity," and "Current Stock Quantity."Inserted a Line Chart:Go to the "Insert" tab on the Excel ribbon.Clicked on "Line" under the "Charts" section.Adjust Chart Design:
I adjust the chart design, titles, and labels as needed for better clarity.

#### Visualization:
The Charts comprises 3 Line-Chart:

i. Current Stock Line Chart
In this chart i highlighted only the order date which is to the x axis and the current stock quantity to the y axis and i beautify the rounded rectangle with some formatting technique.
<img width="318" alt="Current_Stock_Quantity" src="https://github.com/habeebsalaudeen/Tesla-Report-Excel-/assets/97491265/df51e1bb-465d-465a-b25e-9684ac3f8c8d">

ii. Ordered Quantity Line Chart
In this chart I highlighted only the order date which is to the x axis and the order quantity to the y axis and i beautify the rounded rectangle with some formatting technique.
<img width="374" alt="Ordered_Quantity" src="https://github.com/habeebsalaudeen/Tesla-Report-Excel-/assets/97491265/e038089a-d909-4d48-826a-d66f04291a4d">

iii. Current Stock and Ordered Quantity Line Chart 
In this chart i highlighted only the order date which is to the x axis and the current stock quantity and order quantity to the y axis and i beautify the rounded rectangle with some formatting technique.
<img width="623" alt="CurrentStock_Ordered_Quantity" src="https://github.com/habeebsalaudeen/Tesla-Report-Excel-/assets/97491265/3d93148e-9819-48b8-b71e-2cd67c6c2b6a">

#### Whole Report
Whole report of my visualization.
<img width="623" alt="CurrentStock_Ordered_Quantity" src="https://github.com/habeebsalaudeen/Tesla-Report-Excel-/assets/97491265/6058cf03-73a0-4cb8-86d6-8798834dec95">

I Made Chart Dynamic By:
Converting Data to Excel Table 
Press Ctrl + T to convert the range into an Excel Table. 
Define dynamic named ranges for your data. This step is optional but can be helpful.
Go to the "Formulas" tab, click on "Name Manager," and created new named ranges using formulas that automatically adjust to new data in case we have new data.


## Conclusion and Recommendation
The insights generated from the report shows:
- There is a repeated pattern of highest current stock quantity of 342,553 starting from 16th of march 2022
- the highest quantity ordered is 111,770 on 21st of july 2022.
