---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeDateMin Property
nav_order: 171
permalink: /package/extension5/sspread/properties/typedatemin
---
# {{ page.title }}

In the date cell, set the lower limit of the date that can be entered.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeDate (date type).
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties etc. to specify what you want to do.

Specify in YYYYMMDD format. The initial value is "19000101" .

Specify the upper limit with the <a href="/package/extension5/sspread/properties/typedatemax">TypeDateMax</a> property.
The spin button displayed by the <a href="/package/extension5/sspread/properties/typespin">TypeSpin</a> property allows you to increase or decrease the value within the specified range. When the <a href="/package/extension5/sspread/properties/typespinwrap">TypeSpinWrap</a> property is set to $TRUE , the values ​​that have reached the upper and lower limits are wrapped.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> of date type cells.

<a href="/package/extension5/sspread/#precautions-for-specifying-the-range-based-on-the-lower-and-upper-limits-">Points to note when specifying a range using lower and upper limits</a>

Example of use
```
Col = 3;
Row = 2;
CellType = $CellTypeDate;
TypeDateMin = "20000101";
TypeDateMax = "20201231";
Value = str(sysdate(), "YYYYMMDD");
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypeDate;
TypeDateMin = "19500101";
TypeDateMax = "20491231";
Value = str(sysdate(), "YYYYMMDD");
BlockMode = $ FALSE;
```

Related item<br>
 <a href="/package/extension5/sspread/properties/celltype">CellType</a> , <a href="/package/extension5/sspread/properties/typedatemax
 ">TypeDateMax</a> , <a href="/package/extension5/sspread/properties/typespin">TypeSpin</a> , <a href="/package/extension5/sspread/properties/typespinwrap">TypeSpinWrap</a> property