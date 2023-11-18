# Super_Store

![]()

## Introduction

This project is to display my data modelling/dax skills acquired after i concluded a training with Foresight BI under the understanding power Bi. The problem statement is an imaginary case scenario i thought about after seeing the data set. 

## Problem Statement

An international company in the United States wishes to build an headquarter office in the location where the highest sales were made. At the opening event, the takeholders wish to award the customer with the highest sales and also to appoint the best salesrep(i.e the salesrep that has made the highest sales) as a new sales manager of the new headquarter. The stakeholders have hereby entrusted that i carry out analysis and report. 

After thinking critically, some questions need answers:

-  The
-  Which
-  Which

The data set is an excel file saved locally in a folder. The file is denormalised with all data in a single table.

## Data Sourcing

Data was normalised that is, the information was categorically seperated into different sheets or tables resulting into 5 tables:

Sales
Customers
Products
Location
Sales Reps

Data was then locally extracted from Excel Workbook into Power BI for transformation, analysis and visualization.

## Data Transformation

Data cleaning and transformation was carried out using Power Query and it was done per table. After scrutinizing all columns, they were found to be valid and devoid of empty cells and errors. Below is a preview of the tables:

        Products Table                   Customers Table
:--------------------------:|:----------------------------------:

         Locations Table                  Sales Reps
:--------------------------:|:-----------------------------------:

Sales Table
![]()

For the Customers and Products tables, first rows were not headers and so resolved that by applying the "Use First row as header" action. column datatypes were validated appropriately.

## Data Modelling

The data required for this analysis are located in various tables. Therfore, appropriate modelling is required. A star Schema is designed with the Sales Table representing the fact table containing all redundant data, and to which other dimension tables are modelled or connected to using the column that is common. Sales table has been modelledd with:

Customers Table using the "Customer ID"
Products Table using the "Product ID"
Order Rep Table using the "Sale Rep ID"
Locations Table using the "Location ID"

## Data Analysis / Visualization

Before the analysis, it was highly important that i create a Calendar/Date table which is a 'date' format.

Therefore, i created 4 new columns all extracted from the Order data column as my calendar date

-  The first column contained the date this was marked as 'date' format(ie dd/mm/yyy).
-  The second column contains the Month column.
-  Month No was extracted to help with the sorting month hierarchy.
-  The next is the year column
-  The column for quarter was also created.
![]()

Analysis was done using simple visuals since the table have been perfectly modelled together

![]()

Do interact with the dashboard ![here](https://app.powerbi.com/view?r=eyJrIjoiOWM2NzY0ZDMtZWVmNy00M2ZjLTlkNjAtNWE4ZWE2Yzc3N2JmIiwidCI6IjUwODUxMjk2LTliZDEtNGM1Yi05MDllLWY2M2U0OWVmZWEyNSJ9)

![](Customer Overview.png)

Features:
-  Hamburger is a button to display the state and month filter while the red coloured "X" button closes the filter.
-  The five tabs are buttons with hovering effect and each navigate to the page with similar name.

## Analysis

## Customer History
