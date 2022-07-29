---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeCurrencyShowSymbol Property
nav_order: 166
permalink: /package/extension5/sspread/properties/typecurrencyshowsymbol
---
# {{ page.title }}

Set whether to display currency symbols in currency type cells.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeCurrency.
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties etc. to specify what you want to do.

Specify $TRUE if you want to display it, or $FALSE if you do not wish to display it.
The initial value is $TRUE .

The thousands separator can be changed with the <a href="/package/extension5/sspread/properties/typecurrencysymbol">TypeCurrencySymbol</a> property.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> of currency type cells.

Use case
```
Col = 3;
Row = 2;
CellType = $CellTypeCurrency;
TypeCurrencyShowSymbol = $FALSE;
Value = 1.23;
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypeCurrency;
TypeCurrencyShowSymbol = $TRUE;
Value = 4.56;
BlockMode = $FALSE;
```

Related item<br>
 <a href="/package/extension5/sspread/properties/celltype">CellType</a> ,  <a href="/package/extension5/sspread/properties/typecurrencysymbol">TypeCurrencySymbol</a> property