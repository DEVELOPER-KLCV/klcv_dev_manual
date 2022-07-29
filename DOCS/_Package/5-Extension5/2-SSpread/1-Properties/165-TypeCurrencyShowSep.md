---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeCurrencyShowSep Property
nav_order: 165
permalink: /package/extension5/sspread/properties/typecurrencyshowsep
---
# {{ page.title }}

Set whether to display thousands separators in currency type cells.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeCurrency.
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties etc. to specify what you want to process.

Specify $TRUE to display , $FALSE to not display .
The initial value is $FALSE.

The thousands separator can be changed with the <a href="/package/extension5/sspread/properties/typecurrencyshowsep">TypeCurrencySeparator</a> property.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> of currency type cells.

Use case
```
Col = 3;
Row = 2;
CellType = $CellTypeCurrency;
TypeCurrencyShowSep = $TRUE;
Value = 1000000;
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypeCurrency;
TypeCurrencyShowSep = $FALSE;
Value = 1000000;
BlockMode = $FALSE;
```

Related item<br>
 <a href="/package/extension5/sspread/properties/celltype">CellType</a> ,  <a href="/package/extension5/sspread/properties/typecurrencyseparator">TypeCurrencySeparator</a> property