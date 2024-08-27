# Adventure Works Bike Shop Sales Analysis

### Situation
The Sales Department at Adventure Works Bike Shop needed help monitoring and analyzing sales performance across various countries and product lines.

Sales managers required a more dynamic and detailed reporting solution to make data-driven decisions and track performance metrics effectively. The goal was to provide a clear view of sales trends, regional performance, and product profitability.

### Task 
My task was to design and implement a comprehensive sales performance report that would provide insights, facilitate detailed analysis, and support decision-making for the Sales Department.

The objective was to create a Power BI report that included key metrics such as sales by country, product performance, and trend analysis.

### Action
Data Sources: https://github.com/microsoft/powerbi-desktop-samples/blob/main/AdventureWorks%20Sales%20Sample/AdventureWorks%20Sales.xlsx

Data Collection and Preparation: Gathered data from different CSV format files, which consisted of:
- Costumer
- Product
- Reseller
- Sales Territory
- Sales Data
- Sales Order Data
- Date Table

Cleaned the data by checking for missing values and duplicate entries using Power Query.

Data Modeling: Established relationships between tables:
- `fSales_Data` linked to `dCustomer` by `CustomerKey`
- `fSales_Data` linked to `dProduct` by `ProductKey`
- `fSales_Data` linked to `dReseller` by `ResellerKey`
- `fSales_Data` linked to `dSales_Territory` by `SalesTerritoryKey`
- `fSales_Data` linked to `dSales_Order_Data` by `SalesOrderLineKey`
- `fSales_Data` (`OrderDateKey`) linked to `dDate` (`DateKey`)

Metrics and KPIs: Defined and calculated key performance indicators (KPIs) such as Total Revenue, Total Profit, Profit Margin %, Total Cost, Total Units Sold, and Avg. Selling Price.

Report Design: Developed a Power BI report featuring interactive dashboards with visualizations like bar charts, map charts, and matrices to show sales performance across different dimensions. Included slicers and filters to allow users to drill down by country and time period. Designed the report layout to be user-friendly and intuitive, incorporating visual elements that highlighted trends.

### Result
![Sales Dashbaord](https://github.com/angelicamerced/Adventure-Works-Sales-Dashboard/blob/main/Sales%20Dashboard.jpg)

﻿At $51,878,268, FY2020 had the highest Sum of Sales Amount and was 117.42% higher than FY2018, which had the lowest Sum of Sales Amount at $23,860,893.﻿﻿
FY2020 had the highest Sum of Sales Amount at $51,878,268, followed by FY2019 at $34,070,112.67 and FY2018 at $23,860,893.﻿﻿
FY2020 accounted for 47.24% of Sum of Sales Amount.﻿﻿
FY2018 had $23,860,893 Sum of Sales Amount, FY2019 had $34,070,113, and FY2020 had $51,878,268.﻿﻿ 

Total units sold reached 275K, serving a customer base of 18K. The overall profit amounted to $65.8M, resulting in a robust profit margin of 60%. This high profit margin indicates effective cost management and strong sales performance, contributing to a solid financial outcome. The substantial volume of units sold, combined with the high margin, highlights the ability to generate good revenue efficiently.

Bikes have the highest sales, making up 32.83% of the total. Within this category, the Mountain-200 Black, size 38, was the top-selling product. 

The United States was the top performer across all metrics, leading in both revenue and profit, followed by Canada and Australia. Despite its lower revenue ranking, France excelled in profit compared to the United Kingdom, while Germany lagged behind in both profit and profit margin. Notably, Canada boasted the highest profit margin, followed by the United States and France, with Australia having the lowest profit margin.




