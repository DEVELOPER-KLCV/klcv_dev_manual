---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeNumberDecPlaces Property
nav_order: 182
permalink: /package/extension5/sspread/properties/typenumberdecplaces
---
# {{ page.title }}
 
In the numeric cell, set the number of digits to display after the decimal point.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeNumber (numeric type).
<br>Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

You can specify 0 to 14 . The initial value is 2 (digits).

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for numeric cells.

Example of use
```
Col = 3;
Row = 2;
CellType = $ CellTypeNumber;
TypeNumberDecPlaces = 3;
Value = 1.23;
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $ CellTypeNumber;
TypeNumberDecPlaces = 1;
Value = 4.56;
BlockMode = $ FALSE;
 
```

Related item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a>  property