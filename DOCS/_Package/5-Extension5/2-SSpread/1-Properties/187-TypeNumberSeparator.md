---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeNumberSeparator Property
nav_order: 187
permalink: /package/extension5/sspread/properties/typenumberseparator
---
# {{ page.title }}

Set the delimiter every 3 digits in the numeric cell.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeNumber (numeric type).
<br>Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Show / hide the delimiter is set with the <a href="/package/extension5/sspread/properties/typenumbershowsep">TypeNumberShowSep</a> property.
The decimal point symbol is set with the <a href="/package/extension5/sspread/properties/typenumberdecimal">TypeNumberDecimal</a> property.

The initial value is a blank character string ( according to the OS setting value).

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for numeric cells.

Example of use
```
Col = 3;
Row = 2;
CellType = $ CellTypeNumber;
TypeNumberShowSep = $ TRUE;
TypeNumberSeparator = " , ";
Value = 1234.56;
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $ CellTypeNumber;
TypeNumberSeparator = ".";
TypeNumberDecimal = ",";
Value = 1000000;
BlockMode = $ FALSE;
```

Related item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a> , <a href="/package/extension5/sspread/properties/typenumberdecimal">TypeNumberDecimal</a> , <a href="/package/extension5/sspread/properties/typenumbershowsep">TypeNumberShowSep</a> property