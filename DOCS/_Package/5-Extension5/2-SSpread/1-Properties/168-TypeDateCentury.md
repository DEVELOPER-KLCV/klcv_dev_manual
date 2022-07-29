---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeDateCentury Property
nav_order: 168
permalink: /package/extension5/sspread/properties/typedatecentury
---
# {{ page.title }}

In the date cell, set whether to display the year in the Christian era in 4 digits.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeDate (date type).
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties etc. to specify what you want to process.

Specify $TRUE for 4 -digit display and $FALSE for 2 -digit display .
The initial value is the setting value of the OS .

When using two digits for the year , the base year is set with the <a href="/package/extension5/sspread/properties/twodigityearmax">TwoDigitYearMax</a> property.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> of date type cells.

Example of use
```
Col = 3;
Row = 2;
CellType = $CellTypeDate;
TypeDateCentury = $FALSE;
TwoDigitYearMax = 2100; /* 2 digits are in the 2000s * /
Value = str(sysdate(), "YYYYMMDD");
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypeDate;
TypeDateCentury = $ TRUE;
Value = str(sysdate(), "YYYYMMDD");
BlockMode = $FALSE;
```

Related item<br>
 <a href="/package/extension5/sspread/properties/celltype">CellType</a> , <a href="/package/extension5/sspread/properties/typedatecentury">TwoDigitYearMax</a> properties