---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeNumberMax Property
nav_order: 184
permalink: /package/extension5/sspread/properties/typenumbermax
---
# {{ page.title }}

Set the upper limit that can be entered in the numeric cell.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeNumber (numeric type).
<br>Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

The initial value is  9999999.99  .

The lower limit is specified by the <a href="/package/extension5/sspread/properties/typenumbermin">TypeNumberMin</a> property.
The spin button displayed by the <a href="/package/extension5/sspread/properties/typespin">TypeSpin</a> property allows you to increase or decrease the value within the specified range. When the <a href="/package/extension5/sspread/properties/typenspinwrap">TypeSpinWrap</a> property is set to $TRUE , the values ​​that have reached the upper and lower limits are wrapped.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for numeric cells.

<a href="/package/extension5/sspread/#precautions-for-specifying-the-range-based-on-the-lower-and-upper-limits-">Precautions for specifying the range based on the lower and upper limits</a>

Example of use
```
Col = 3;
Row = 2;
CellType = $ CellTypeNumber;
TypeNumberMin = 0;
TypeNumberMax = 100;
Value = 0;
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $ CellTypeNumber;
TypeNumberMin = -100;
TypeNumberMax = 100;
Value = 0;
BlockMode = $ FALSE;
```

Related item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a> , <a href="/package/extension5/sspread/properties/typenumbermin">TypeNumberMin</a> , <a href="/package/extension5/sspread/properties/typespin">TypeSpin</a> , <a href="/package/extension5/sspread/properties/typenspinwrap">TypeSpinWrap</a> property