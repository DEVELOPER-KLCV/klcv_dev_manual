---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeScientificMax Property
nav_order: 203
permalink: /package/extension5/sspread/properties/typescientificmax
---
# {{ page.title }}

In the exponential cell, set the lower limit that can be input.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeScientific.
<br>Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

The initial value is -1.7E + 308 .

The upper limit is specified by the <a href="/package/extension5/sspread/properties/typescientificmin">TypeScientificMin </a> property.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for exponential cells .

<a href="/package/extension5/sspread/#precautions-for-specifying-the-range-based-on-the-lower-and-upper-limits-">Precautions for specifying the range based on the lower and upper limits.</a>

Example of use
```
Col = 3;
Row = 2;
CellType = $CellTypeScientific;
TypeScientificDecPlaces = 2;
TypeScientificMin = 0;
TypeScientificMax = 1000000;
Value = 0;
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypeScientific;
TypeScientificMin = -1000000;
TypeScientificMax = 1000000;
Value = 0;
BlockMode = $FALSE;
```

Related item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a> , <a href="/package/extension5/sspread/properties/typescientificmin">TypeScientificMin</a> property