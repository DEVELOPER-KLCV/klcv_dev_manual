---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeNumberShowSep Property
nav_order: 188
permalink: /package/extension5/sspread/properties/typenumbershowsep
---
# {{ page.title }}

Set whether to display the delimiter every 3 digits in the numeric cell.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeNumber (numeric type).
<br>Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Specify $TRUE if you want to display it, or $FALSE if you do not want to display it.
The initial value is $FALSE .

The delimiter for every 3 digits can be changed with the <a href="/package/extension5/sspread/properties/typenumberseparator">TypeNumberSeparator</a> property.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for numeric cells.

Example of use
```
Col = 3;
Row = 2;
CellType = $ CellTypeNumber;
TypeNumberShowSep = $ TRUE;
Value = 1000000;
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $ CellTypeNumber;
TypeNumberShowSep = $ FALSE;
Value = 1000000;
BlockMode = $ FALSE;
```

Related item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a> , <a href="/package/extension5/sspread/properties/typenumberseparator">TypeNumberSeparator</a> property