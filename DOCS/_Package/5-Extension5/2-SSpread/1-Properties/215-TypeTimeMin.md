---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeTimeMin Property
nav_order: 215
permalink: /package/extension5/sspread/properties/typetimemin
---
# {{ page.title }}

In the time cell, set the lower limit of the date that can be entered.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $ CellTypeTime .
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Specify format is in HHMMSS. The initial value is "000000" .

The lower limit is specified by the <a href="/package/extension5/sspread/properties/typetimemax">TypeTimeMax</a> property.
The spin button displayed by the <a href="/package/extension5/sspread/properties/typespin">TypeSpin</a> property allows you to increase or decrease the value within the specified range. When the  <a href="/package/extension5/sspread/properties/typespinwrap">TypeSpinWrap</a> property is set to $ TRUE , the values ​​that have reached the upper and lower limits are wrapped.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for time cells .

<a href="/package/extension5/sspread/#precautions-for-specifying-the-range-based-on-the-lower-and-upper-limits-">Precautions for specifying the range by the lower limit value and upper limit value</a>

Example of use
```
Col = 3;
Row = 2;
CellType = $ CellTypeTime;
TypeTimeMin = "080000";
TypeTimeMax = "205959";
Value = str (sysdate (), "HHMISS");
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $ CellTypeTime;
TypeTimeMin = "060000";
TypeTimeMax = "225959";
Value = str (sysdate (), "HHMISS");
BlockMode = $ FALSE;
```

Related item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a> , <a href="/package/extension5/sspread/properties/typetimemax">TypeTimeMax</a> , <a href="/package/extension5/sspread/properties/typespinwrap">TypeSpin</a> , <a href="/package/extension5/sspread/properties/celltype">TypeSpinWrap</a> properties

