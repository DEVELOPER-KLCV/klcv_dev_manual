---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeCurrencySeparator Property
nav_order: 164
permalink: /package/extension5/sspread/properties/typecurrencyseparator
---
# {{ page.title }}

Set the thousands separator in currency type cells.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeCurrency(currency type).
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties etc. to specify what you want to process.

The initial value is a blank string ( according to OS settings).

Show / hide the delimiter is set with the <a href="/package/extension5/sspread/properties/typecurrencyshowsep">TypeCurrencyShowSep</a> property.
Set the decimal symbol with the <a href="/package/extension5/sspread/properties/typecurrencydecimal">TypeCurrencyDecimal</a> property and the currency symbol with the <a href="/package/extension5/sspread/properties/typecurrencysymbol">TypeCurrencySymbol</a> property.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> of currency type cells.

Use case
```
Col = 3;
Row = 2;
CellType = $CellTypeCurrency;
TypeCurrencyShowSep = $TRUE;
TypeCurrencySeparator = "，";
Value = 1234.56;
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypeCurrency;
TypeCurrencySeparator = ".";
TypeCurrencyDecimal = ",";
Value = 1000000;
BlockMode = $FALSE;
```

Related item<br>
 <a href="/package/extension5/sspread/properties/celltype">CellType</a> ,  <a href="/package/extension5/sspread/properties/typecurrencydecimal">TypeCurrencyDecimal</a> ,  <a href="/package/extension5/sspread/properties/typecurrncyshowsep">TypeCurrencyShowSep</a> ,  <a href="/package/extension5/sspread/properties/typecurrencysymbol">TypeCurrencySymbol</a> property
 