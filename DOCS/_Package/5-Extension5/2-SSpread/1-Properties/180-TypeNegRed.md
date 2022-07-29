---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeNegRed Property
nav_order: 180
permalink: /package/extension5/sspread/properties/typenegred
---
# {{ page.title }}

Set whether to display negative numbers in red.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property.
<br>$CellTypeCurrency
<br>$CellTypeNumber
<br>$CellTypePercent
<br>$CellTypeScientific

Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Specify $TRUE to display negative numbers in red, otherwise $FALSE .
The initial value is $FALSE .

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for data type cell.

Example of use
```
Col = 3;
Row = 2;
CellType = $CellTypeNumber;
TypeNegRed = $TRUE;
Value = -123;
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypePercent;
TypeNegRed = $TRUE;
Value = -0.123;
BlockMode = $FALSE; 
```

Related item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a> , <a href="/package/extension5/sspread/properties/typencurrencynegstyle">TypeCurrencyNegStyle</a> , <a href="/package/extension5/sspread/properties/typenumbernegstyle">TypeNumberNegStyle</a>,  <a href="/package/extension5/sspread/properties/typepercentnegstyle">TypePercentNegStyle</a> property