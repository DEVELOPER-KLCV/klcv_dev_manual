---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeCurrencyDecPlaces Property
nav_order: 158
permalink: /package/extension5/sspread/properties/typecurrencydecplaces
---
# {{ page.title }}

In the currency cell, set the number of digits to display after the decimal point.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeCurrency (currency type).
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties etc. to specify what you want to process.

You can specify 0 to 14 . The initial value is 2 (digits).

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> of currency type cells.

Example of use
```
Col = 3;
Row = 2;
CellType = $ CellTypeCurrency;
TypeCurrencyDecPlaces = 3;
Value = 1.23;
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $ CellTypeCurrency;
TypeCurrencyDecPlaces = 1;
Value = 4.56;
BlockMode = $ FALSE;
```

Related item<br>
 <a href="/package/extension5/sspread/properties/celltype">CellType</a> property
 