# Coffee-Sales-Dashboard-Data-Analytics-by-Excel
![](coffee_store.jpg)
---

## Introduction
This Coffee Sales dashboard was created to help Manager investigate sales of coffee,by Coffee name, country and by Customers names.
The data is from my Excel document, which provides a foundation in analyzing data using this powerful tool. The data contains detailed information on Order ID,Customer ID,Customer Name,Coffee Type Name etc and essential skills that are presented here.

## Dashboard File
My final [dashboard](https://github.com/Othmane-data/Coffee-Sales-Dashboard-by-Excel/blob/main/coffeeOrdersData.xlsx)

## Problem statement
1. What is the total sales of coffee by years ,mounths and Coffee type name?
2. What is the top sales of Coffee in dollars,by Country?
3. What is the top 5 sales of Coffee by Customers name?

## Skills/ concepts demonstrated
- 🧮 Formulas and Functions
- 📉 Charts and Visualization
- ❎ Data Validation

  ```
  =IF
  (XLOOKUP(C2,customers!$A$1:$A$1001,customers!$C$1:$C$1001,,0)=0,"",
  XLOOKUP(C2,customers!$A$1:$A$1001,customers!$C$1:$C$1001,,0))
  ```



