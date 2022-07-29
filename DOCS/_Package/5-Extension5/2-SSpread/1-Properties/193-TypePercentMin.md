---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypePercentMin Property
nav_order: 193
permalink: /package/extension5/sspread/properties/typepercentmin
---
# {{ page.title }}

Set the lower limit that can be entered in the percentage cell.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $ CellTypePercent (percentage type).
<br>Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

The initial value is -9999.99 .

The upper limit is specified by the <a href="/package/extension5/sspread/properties/typepercentmax">TypePercentMax</a> property.
The spin button displayed by the <a href="/package/extension5/sspread/properties/typespin">TypeSpin</a> property allows you to increase or decrease the value within the specified range. When the <a href="/package/extension5/sspread/properties/typespinwrap">TypeSpinWrap</a> property is set to $TRUE , the values ​​that have reached the upper and lower limits are wrapped.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for percentage cells.

<a href="/package/extension5/sspread/#precautions-for-specifying-the-range-based-on-the-lower-and-upper-limits-">Precautions for specifying the range based on the lower and upper limits</a>

Example of use
```
Col = 3;
Row = 2;
CellType = $ CellTypePercent;
TypePercentMin = 0;
TypePercentMax = 100;
Value = 0;
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $ CellTypePercent;
TypePercentMin = -100;
TypePercentMax = 100;
Value = 0;
BlockMode = $ FALSE;
```

Related item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a>, <a href="/package/extension5/sspread/properties/typepercentmax">TypePercentMax</a>, <a href="/package/extension5/sspread/properties/typespin">TypeSpin</a>, <a href="/package/extension5/sspread/properties/typespinwrap">TypeSpinWrap</a> properties.