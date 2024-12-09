# Seven Sages Brewing Company

## Project Overview

The primary focus of this project is on data preparation and modeling using Power BI. 


## Project Description

The project is about creating a comprehensive data model and Power BI report for Seven Sages Brewing Company, a fictional entity really. The main objective is to develop a tool that enables the company's CFO to efficiently analyze beer sales performance and profitability.


## Data Sources

The source material for this project can be found under the folder called “Source files”.

* Promotional document(Product Offerings `PDF`): The sales department has provided a promotional document that lists all the company’s current offerings, ratings, and servings sizes.

* Purchases(Monthly Sales Logs `folder`): An operations assistant has provided data on purchases for 'EVERY MONTH', in the form of `multiple Excel spreadsheets`

* Customer records(Customer List (as of FY2021).`txt`): Text file IT provided regarding customer records. They had to download these separately, but they have assured us that they are up to date.

* Metrics documentation(CFO Metrics Tracker.`xlsx`): The CFO has provided her metrics documentation that she’s been compiling on sales, costs, and servings (per item for sael)

* USD-CAD Exchange Rates `csv`: CSV file for currency excahnge accross both regions of company operations

## Data Model 

![Data Model](Screenshots/Screenshot%202024-12-06%20at%2005.34.30.png)

* Fact Table:
  1. Monthly sales logs
 
* Dimension Tables:
  1. Product offerings
  2. Customers list
  3. Date
  4. USD-CAD Exchange Rates

* Measures:
  1. Sales USD
  2. Sales CAD
  3. Cost of Sales
  4. Gross Profit Margin
  5. Unit Sales by Product
  6. Gross Profit by Product
 
### Date Table Creation
A dynamic date table that starts at the beginning of the calendar year(`Start`) and ends at the end of the calendar year(`End`) as seen in the model diagram above was created from the Monthly Sales Logs folders(combined into a .xlsx file eventually)

The following extra fields were created:

* Calendar Month Number and Name
* Calendar Year
* Fiscal Period
* Fiscal Year
* Fiscal Quarter (example: Q2-FY2020)
(Seven Sages’ Fiscal year begins on October 1st and runs until September 30th. )


## Modelling Results

Table #1
![Table1](Screenshots/Screenshot%202024-12-07%20at%2002.26.14.png)
* This table summarised the Sales for each Customer type across different quarters of the year.

Table #2
![Table2](Screenshots/Screenshot%202024-12-07%20at%2002.26.35.png)
* THis sumarised percentages of gross profit and unit sales by products. The executive summary gives more insight into everything.

## Summary
* All extra details needed are in the `ayo.pbix` sheet. This includes the data modelling, dimensions & measures creations, everything, reference it for more info if needed
* The `Reports.pdf` is the report pdf published to my PBI Service


## Licensing
This project is for personal and educational purposes, feel free to copy/use it
