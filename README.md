# Café Sales Analysis: Power BI Dashboard

## 1. Problem statement
A café wants to understand its 2023 sales performance: which items drive revenue, when sales peak, how customers pay and where they buy, and what should be improved. This project cleans the transaction data, analyses it and presents the findings in an interactive dashboard.

## 2. Dataset
- Source: café transaction data (file: `cafe_sales_cleaned.csv`)
- Size: 9,064 transactions, 1 Jan 2023 to 31 Dec 2023
- Columns: Transaction ID, Item, Quantity, Price Per Unit, Total Spent, Payment Method, Location, Transaction Date, Month, Weekday
- Items: Cake, Coffee, Cookie, Juice, Salad, Sandwich, Smoothie, Tea

## 3. Data cleaning
- Checked for missing values and duplicate Transaction IDs: none remain
- Converted Transaction Date to a proper date type
- Added Month and Weekday columns from the date
- Kept missing payment method and location values as "Unknown" instead of deleting rows, so revenue totals stay complete

## 4. Analysis
Done in Excel (`cafe_sales_analysis.xlsx`: Summary, Item Analysis, Trends, Payment & Location, Insights sheets) and Power BI (DAX measures: Total Revenue, Total Transactions, Total Items Sold, Avg Order Value; Calendar table linked to Transaction Date).

## 5. Dashboard
![Dashboard](Screenshot%202026-10-17%20230820.png)

- KPIs: Revenue, Transactions, Average Order Value, Items Sold
- Charts: revenue by month, item, weekday, payment method, location
- Filters (slicers): Item, Payment Method

## 6. Key business insights
- Total revenue is about $80,042 from 9,064 transactions; average order value is $8.83 and 27,358 items were sold.
- Salad (about 23%), Sandwich and Smoothie together bring in about 55% of revenue.
- Tea and Cookie are the lowest earners (about $5.2K and $3.4K), partly because of their low prices ($1.50 and $1).
- Sales are steady through the year (about $6.2K to $7.0K per month). October is highest and February lowest.
- Thursday is the strongest weekday and Wednesday the weakest, but the gap is small (about 8%).
- Cash, Credit Card and Digital Wallet are used almost equally.
- About 31% of revenue has no recorded payment method and about 40% has no recorded location, so payment and location analysis is only partial.

## 7. Recommendations
- Promote top items and bundle them with low earners (for example Salad or Sandwich with Cookie or Tea).
- Run a mid-week offer to lift Wednesday sales.
- Make payment method and location mandatory in the billing system to fix the data gap.

## 8. Tools
Excel, Power BI (DAX, data modelling)

## Files
- `cafe_sales_cleaned.csv`: cleaned dataset
- `cafe_sales_analysis.xlsx`: analysis workbook
- Dashboard screenshot (above)
