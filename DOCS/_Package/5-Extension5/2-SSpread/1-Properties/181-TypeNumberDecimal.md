---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeNumberDecimal Property
nav_order: 181
permalink: /package/extension5/sspread/properties/typenumberdecimal
---
# {{ page.title }}

Set the decimal point symbol in the numeric cell.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeNumber (numeric type).
<br>Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

The initial value is a blank character string ( according to the OS setting value).


The number of digits after the decimal point is set with the <a href="/package/extension5/sspread/properties/typenumberdecplaces">TypeNumberDecPlaces</a> property.
The delimiter for every 3 digits is set with the <a href="/package/extension5/sspread/properties/typenumberseparator">TypeNumberSeparator</a> property.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for numeric cells.

Example of use
```
Col = 3;
Row = 2;
CellType = $ CellTypeNumber;
TypeNumberDecimal = "・";
Value = 1.23;
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $ CellTypeNumber;
TypeNumberDecimal = ",";
Value = 4.56;
BlockMode = $ FALSE;
 
```

Related item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a> , <a href="/package/extension5/sspread/properties/typenumberdecplaces">TypeNumberDecPlaces</a> , <a href="/package/extension5/sspread/properties/typenumberseparator">TypeNumberSeparator</a>   property