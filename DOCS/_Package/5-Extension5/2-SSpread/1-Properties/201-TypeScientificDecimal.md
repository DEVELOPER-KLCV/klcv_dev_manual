---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeScientificDecimal Property
nav_order: 201
permalink: /package/extension5/sspread/properties/typescientificdecimal
---
# {{ page.title }}
Set the decimal point symbol in the exponential cell.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeScientific.
<br>Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

The initial value is a blank character string ( according to the OS setting value).

The number of digits after the decimal point is set with the <a href="/package/extension5/sspread/properties/typescientificdecplaces">TypeScientificDecPlaces</a> property.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for exponential cells .

Example of use
```
Col = 3;
Row = 2;
CellType = $ CellTypeScientific;
TypeScientificDecPlaces = 3;
Value = 0.1234;
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $ CellTypeScientific;
TypeScientificDecPlaces = 1;
Value = 0.5678;
BlockMode = $ FALSE;
```

Related item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a>, <a href="/package/extension5/sspread/properties/typescientificdecplaces">TypeScientificDecPlaces</a> property.