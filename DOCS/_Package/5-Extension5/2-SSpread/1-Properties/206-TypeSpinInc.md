---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeSpinInc Property
nav_order: 206
permalink: /package/extension5/sspread/properties/typespininc
---
# {{ page.title }}

Sets the amount of change due to a single click of the spin button displayed in the cell .

Only valid for cells with the following values ​​set in the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property.
<br>$CellTypeCurrency (currency type)
<br>$CellTypeNumber (number type)
<br>$CellTypePercent (percent type)

Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

When the cursor is in the integer part, the value of the integer part of the number set in this property increases or decreases.
When the cursor is in the fractional part, the value of the decimal part of the number set in this property increases or decreases.
The initial value is 1.1 (integer increment is 1 and fractional increment is 0.1 ).

The spin button is displayed when the <a href="/package/extension5/sspread/properties/typespin">TypeSpin</a> property is set to $TRUE .

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for each data type cells .

Example of use
```
Col = 3;
Row = 2;
CellType = $ CellTypeNumber;
TypeSpin = $ TRUE;
TypeSpinInc = 2.2;
TypeSpinWrap = $ TRUE;
TypeNumberMin = 0;
TypeNumberMax = 10;
Value = 0;
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $ CellTypeCurrency;
TypeSpin = $ TRUE;
TypeSpinInc = 100.0;
TypeCurrencyDecPlaces = 0;
Value = 0;
BlockMode = $ FALSE;
```

Related item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a> , <a href="/package/extension5/sspread/properties/typespin">TypeSpin</a>  , <a href="/package/extension5/sspread/properties/typespinwrap">TypeSpinWrap</a> property