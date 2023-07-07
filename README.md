# Power BI Report for Forggith Pharmaceuticals

## Introduction

![](https://github.com/TheGreatFateemah/Forggith-Pharmaceuticals/blob/main/Forggith.jpg)

Forggith Pharmaceuticals is a Pharmaceutical Manufacturing company based in Germany. The project is a Power BI report that shows the sales and marketing performance overview of the pharmaceutical company. The project is to guide their strategies, tactics, and operations as a company.

## Problem Statement

1.	What is the total revenue and total target?
2.	Which channel generated the highest revenue?
3.	What is the total revenue Year to Date (YTD) and total target Year to Date (YTD)
4.	Which product class have the highest revenue?
5.	Which sales rep and sales team generated the highest revenue?
6.	Which sales rep achieve the highest volume.
7.	Which sales rep have the highest target?
8.	Top 5 products that have the highest volume.

## Skills/Concept Demonstrated

-	Data Dictionary creation
-	Power Query
-	Data modelling
-	Data Analysis Expression (DAX)
-	Data visualization

## Data Transformation

The original dataset contains eight tables:
1.	Targets
2.	DimLocation
3.	DimSubChannel
4.	DimChannel
5.	DimProducts
6.	DimEmployees
7.	Sales2022
8.	Sales2023-2025

During transformation process,
1.	I used the append queries function to append Sales2022 and Sales2023-2025 tables into a single table that I named Sales2022-2025F
2.	I used the merge queries function to merge DimChannel and DimSubChannel tables with a matching column (ChannelID) into a single table that I named DimChannel&SubChannel
3.	I created a column for Revenue in the Sales2022-2025F table which multiplies Product Price by Quantity.
4.	I created a calendar table that contains Date, Year, Quarter, Month and Month No.
5.	I created DAX measure for:
-	Total Revenue
-	Total Target
-	Revenue Year to Date (YTD)
-	Revenue Same Period Last Year (SPLY)
-	Target YTD
-	Target Previous Year YTD
-	Previous Year Revenue YTD
-	Revenue % change

## Modelling
There are two Fact tables (Sales2022-2025F and Targets), four Dimension tables (DimProduct, DimEmployees, DimLocation, DimChannel&SubChannel) and one Calendar table.

![](https://github.com/TheGreatFateemah/Forggith-Pharmaceuticals/blob/main/Model.jpg)

## Visualization

The report consists of three pages:
1.	Home page where you can navigate to the sales and marketing performance overview pages.
2.	Sales Performance Overview.
3.	Marketing Performance Overview.

You can interact with the report [here](https://app.powerbi.com/view?r=eyJrIjoiMmIxNGIyYjctNDczMS00Y2RjLWEyZmUtMDZiM2RiNzZhYmE5IiwidCI6IjA1MDk5ZmE3LWZlMDYtNGE0ZC04MDc5LTNjNDI1ZmU4NzM0YiJ9)

## Analysis

**Note:** I used February 2024 as the default slicer because there are YTD charts in the report, so these analyses are based on February 2024

![](https://github.com/TheGreatFateemah/Forggith-Pharmaceuticals/blob/main/Sales.jpg)

-	Total Revenue is approximately 289million.
-	Total Target is approximately 446thousand.
-	Pharmacy generated the highest revenue.
-	Total Revenue YTD is approximately 386million.
- Total Target YTD is approximately 891thousand.
-	Antimalarial drugs had the highest revenue.

![](https://github.com/TheGreatFateemah/Forggith-Pharmaceuticals/blob/main/Marketing.jpg)

-	Abigail Thompson generated the highest revenue and volume.
-	Delta team generated the highest revenue.
-	Anne Wu had the highest target.
-	Limoulin, Araxetine, Ribabyclor, Ceftatana, Serolamide and Propratecan had the highest volume.

## Conclusion and Recommendations

This is also based on the data for Feb,2023.
1.	The company should look for all possible means to retain Abigail Thompson either by giving out incentives or an increase in pay.
2.	The company can also work more with the Koss distributors.
3.	The Delta team also did well and should be rewarded.









