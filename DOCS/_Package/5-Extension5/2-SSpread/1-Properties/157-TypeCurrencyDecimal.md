---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeCurrencyDecimal Property
nav_order: 157
permalink: /package/extension5/sspread/properties/typecurrencydecimal
---
# {{ page.title }}

Set the decimal point symbol in the currency cell.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeCurrency (currency type).
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties etc. to specify what you want to do.

The initial value is a blank string ( according to OS settings).

Set the number of decimal places with the <a href="/package/extension5/sspread/properties/typecurrencydecplaces">TypeCurrencyDecPlaces</a> property.
<br>Set the thousands separator with the <a href="/package/extension5/sspread/properties/typecurrencyseparator">TypeCurrencySeparator</a> property and the currency symbol with the <a href="/package/extension5/sspread/properties/typecurrencysymbol">TypeCurrencySymbol </a> property.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> of currency cells.

Example of use
```
Col = 3;
Row = 2;
CellType = $CellTypeCurrency;
TypeCurrencyDecimal = "・";
Value = 1.23;
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypeCurrency;
TypeCurrencyDecimal = ",";
Value = 4.56;
BlockMode = $ FALSE;
```

Related item<br>
 <a href="/package/extension5/sspread/properties/celltype">CellType</a> , <a href="/package/extension5/sspread/properties/typecurrencydecplaces">TypeCurrencyDecPlaces</a> , <a href="/package/extension5/sspread/properties/typecurrencyseparator">TypeCurrencySeparator</a> , <a href="/package/extension5/sspread/properties/typecurrencysymbol">TypeCurrencySymbol </a> properties