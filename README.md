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
- ❎ Data Validation


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


