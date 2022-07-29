---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeSpinWrap Property
nav_order: 207
permalink: /package/extension5/sspread/properties/typespinwrap
---
# {{ page.title }}

With the spin button displayed in the cell, set the operation when the set upper limit value and lower limit value are reached.

Only valid for cells with the following values ​​set in the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property.
<br>$CellTypeCurrency
<br>$CellTypeNumber
<br>$CellTypePercent

Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Specify $TRUE if you want to wrap the value, or $FALSE if you do not want to change the value .
The initial value is $FALSE .

The spin button is displayed when the <a href="/package/extension5/sspread/properties/typespin">TypeSpin</a> property is set to $TRUE .

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for each data type cells .

Example of use
```
Col = 3;
Row = 2;
CellType = $ CellTypeNumber;
TypeSpin = $ TRUE;
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
TypeSpinWrap = $ TRUE;
TypeCurrencyMin = 0;
TypeCurrencyMax = 500;
TypeCurrencyDecPlaces = 0;
Value = 0;
BlockMode = $ FALSE;
```

Related item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a> , <a href="/package/extension5/sspread/properties/typespin">TypeSpin</a>  , <a href="/package/extension5/sspread/properties/typespininc">TypeSpinInc</a> property