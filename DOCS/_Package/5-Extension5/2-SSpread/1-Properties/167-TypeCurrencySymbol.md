---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeCurrencySymbol Property
nav_order: 167
permalink: /package/extension5/sspread/properties/typecurrencysymbol
---
# {{ page.title }}

Set the currency symbol in a currency type cell.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeCurrency (currrency type).
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties etc. to specify what you want to do.

The initial value is a blank string ( according to OS settings).

Show / hide the currency symbol with the <a href="/package/extension5/sspread/properties/typecurrencysymbol">TypeCurrencyShowSymbol</a> property.
Set the decimal separator in the <a href="/package/extension5/sspread/properties/typecurrencydecimal">TypeCurrencyDecimal</a>  property and the thousands separator in the <a href="/package/extension5/sspread/properties/typecurrencyseparator">TypeCurrencySeparator</a> property.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> of currency type cells.

Example of use
```
Col = 3;
Row = 2;
CellType = $CellTypeCurrency;
TypeCurrencySymbol = "$";
Value = 1.23;
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypeCurrency;
TypeCurrencySymbol = "￡";
Value = 4.56;
BlockMode = $FALSE;
```

Related item<br>
 <a href="/package/extension5/sspread/properties/celltype">CellType</a> , <a href="/package/extension5/sspread/properties/typecurrencydecimal">TypeCurrencyDecimal</a> , <a href="/package/extension5/sspread/properties/typecurrencyseparator">TypeCurrencySeparator</a> , <a href="/package/extension5/sspread/properties/typecurrencyshowsymbol">TypeCurrencyShowSymbol </a> properties
