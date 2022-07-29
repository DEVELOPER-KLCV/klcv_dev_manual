---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeSpin Property
nav_order: 205
permalink: /package/extension5/sspread/properties/typespin
---
# {{ page.title }}

Set whether to display the spin button in the cell.

Only valid for cells with the following values ​​set in the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property.
<br>$CellTypeDate (date type)
<br>$CellTypeTime (time type)
<br>$CellTypeCurrency (currency type)
<br>$CellTypeNumber (numerical type)
<br>$CellTypePercent (percent type)

Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Specify $TRUE if want the spin button to appear, or else, $FALSE if don't want the button to appear.
The initial value is $FALSE .


The spin button is displayed when the cell is in input mode ( <a href="/package/extension5/sspread/properties/editmode">EditMode</a> property is $ TRUE ).
The user can increase or decrease the value by clicking a button.

You can specify the <a href="/package/extension5/sspread/properties/typespininc">TypeSpinInc</a>, <a href="/package/extension5/sspread/properties/typespinwrap">TypeSpinWrap</a> properties for currency, number, and percentage cells .
The TypeSpinInc property sets the amount of change in the value with a single click, and the TypeSpinWrap property sets the behavior when the upper and lower limits of the cell are reached.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for each data type cell .

Example of use
```
Col = 3;
Row = 2;
CellType = $ CellTypeDate;
TypeSpin = $ TRUE;
Value = str (sysdate (), "YYYYMMDD");
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $ CellTypeNumber;
TypeSpin = $ TRUE;
Value = 0;
BlockMode = $ FALSE;
```

Related item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a> , <a href="/package/extension5/sspread/properties/typespininc">TypeSpinInc</a>  , <a href="/package/extension5/sspread/properties/typespinwrap">TypeSpinWrap</a> property