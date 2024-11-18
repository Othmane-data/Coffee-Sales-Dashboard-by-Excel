# Coffee-Sales-Dashboard-Data-Analytics-by-Excel
![](coffee_store.jpg)
---

## Introduction
This Coffee Sales dashboard was created to help ManagerS investigate sales of coffee,by Coffee name, country and, by Customers names.
The data is from my Excel document, which provides a foundation in analyzing data using this powerful tool. The data contains detailed information on Order ID,Customer ID,CustomerS Name,Coffee Type Name etc and essential skills that are presented here.

## Dashboard File
My final [dashboard](https://github.com/Othmane-data/Coffee-Sales-Dashboard-by-Excel/blob/main/coffeeOrdersData.xlsx)

## Problem statement
1. What is the total sales of coffee by years ,mounths and Coffee type name?
2. What is the top sales of Coffee in dollars,by Country?
3. What is the top 5 sales of Coffee by Customers name?

## Skills/ concepts demonstrated
- 🧮 Formulas and Functions
- 📉 Charts and Visualization
- ❎ Conclusion and Recommendations


### 🧮 Formulas and Functions:
- Customer Name,Email,Country;
```
- Customer Name=XLOOKUP
  (C2,customers!$A$1:$A$1001,
    customers!$B$1:$B$1001,,0)
  
- Email=IF
  (XLOOKUP(C2,customers!$A$1:$A$1001,
    customers!$C$1:$C$1001,,0)=0,"",
      XLOOKUP(C2,customers!$A$1:$A$1001,customers!$C$1:$C$1001,,0))

- Country=XLOOKUP
  (C2,customers!$A$1:$A$1001,
    customers!$G$1:$G$1001,,0)
```
  
- Coffee Type,Roast Type,Unit Price;
```
- Coffee Type=INDEX
(products!$A$1:$G$49,
  MATCH(orders!$D2,products!$A$1:$A$49,0),
    MATCH(products!$B$1,products!$A$1:$G$1,0))

-Roast Type=INDEX
(products!$A$1:$G$49,
  MATCH(orders!$D2,products!$A$1:$A$49,0),
    MATCH(products!$C$1,products!$A$1:$G$1,0))

-Unit Price==INDEX
(products!$A$1:$G$49,
  MATCH(orders!$D2,products!$A$1:$A$49,0),
    MATCH(products!$E$1,products!$A$1:$G$1,0))
```

### 📉 Charts and Visualization:
The report comprises 3 charts:

___1. Top Sales Of Coffee;___

___2. Top Sales By Country;___

___3. Top Sales By Customers Name.___

we're use the pivot table for every shart

__- Features:__
- Order Date by Mounth Timeline;
- Size Slicer;
- Roast Type Name Slicer;
- Loyalty Card Slicer.

You can view the all dashboard [here](coffeeOrdersData.xlsx)

___1. Top Sales Of Coffee:___

![](total_of_coffee.png)

analyser cettebshart

___2. Top Sales By Country:___

![](top_sales_by_country.PNG)

analyser cettebshart

___3. Top Sales By Customers Name:___

![](top_sales_by_customers_name.PNG)

analyser cettebshart



### ❎ Conclusion and Recommendations:
