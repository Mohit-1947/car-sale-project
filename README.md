# car sales project

# Car Sales Report — Power BI Dashboard

## Overview
This project uses the [Car Sales Data](https://www.kaggle.com/datasets/suraj520/car-sales-data) dataset from Kaggle, containing approximately 2.5 million car sales records across multiple car makes and models, sales persons, and years (2022–2023). Unlike prior projects, this dataset was already clean — the focus here was on building DAX measures from scratch, designing a clean visual layout, and adding interactive filtering (slicers) to make the dashboard genuinely explorable, rather than static.

## Dataset
- Source: [Car Sales Data (Kaggle)](https://www.kaggle.com/datasets/suraj520/car-sales-data)
- ~2.5 million rows of car sales transactions
- Fields include Car Make, Car Model, Sale Price, Commission Earned, Sales Person, and Year

## Key DAX Measures
- total sales = SUM(car_sales_data[Sale Price])
- number of sales = COUNTROWS(car_sales_data)
- Total Commission Earned = SUM(car_sales_data[Commission Earned])

These three measures form the KPI cards at the top of the dashboard and recalculate dynamically based on whichever slicers are active.

## Interactive Slicers
- Car Make — button-style slicer (Chevrolet, Ford, Honda, Nissan, Toyota)
- Year — checkbox slicer (2022, 2023)
- Sales Person — searchable list slicer, allowing filtering by individual salesperson name

Adding slicers this time was a deliberate shift from the earlier static dashboards — it lets a user drill into a specific make, year, or salesperson and see every KPI and chart update accordingly, rather than only viewing one fixed view of the data.

## Dashboard Features
- KPI cards: Sum of Sale Price, Number of Sales, Total Commission Earned
- Number of sales by Car Model (donut chart)
- Sum of Commission Earned by Car Make (bar chart)
- Total sales by Month (column chart)
- Detailed transaction table (Total Sales, Car Model, Year, Number of Sales)

## Tools Used
Power BI, DAX


