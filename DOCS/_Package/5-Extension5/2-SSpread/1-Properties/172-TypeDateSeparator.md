---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeDateSeparator Property
nav_order: 172
permalink: /package/extension5/sspread/properties/typedateseparator
---
# {{ page.title }}

Set the year-month-day separator in a date type cell.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeDate (date type).
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties etc. to specify what you want to process.

The delimiter specifies the Unicode character code as a number. Set to 47 ( 0x2F , '/' ) if you want to use forward slashes .
Do not specify illegal characters that cannot be displayed correctly, such as control characters and special characters.

If set to 63 ( 0x3F , '?' ), "year, month, day" will be the delimiter. If 0 is set, the OS setting value is set.

The initial value is the OS setting value.
The date format is set with the <a href="/package/extension5/sspread/properties/typedateformat">TypeDateFormat</a> property.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> of date type cells.

Use case
```
Col = 3;
Row = 2;
CellType = $CellTypeDate;
TypeDateSeparator = 0x3F; / *'?' * /
Value = str(sysdate(), "YYYYMMDD");
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypeDate;
TypeDateSeparator = 0x2D; /* '-' */
Value = str(sysdate(), "YYYYMMDD");
BlockMode = $ FALSE;
```

Related item<br>
 <a href="/package/extension5/sspread/properties/celltype">CellType</a> , <a href="/package/extension5/sspread/properties/typedateformat
 ">TypeDateFormat</a> property