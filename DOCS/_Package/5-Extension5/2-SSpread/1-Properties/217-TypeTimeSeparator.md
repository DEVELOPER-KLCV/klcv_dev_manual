---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeTimeSeparator Property
nav_order: 217
permalink: /package/extension5/sspread/properties/typetimeseparator
---
# {{ page.title }}

 To set the hour, minute, and second delimiters in the time cell.

Only valid for cells with the 
<a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $ CellTypeTime .
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

For the delimiter , specify the Unicode character code as a numerical value. If you want to use a colon, set it to 58 ( 0x3A , ':' ).
Do not specify illegal characters that cannot be displayed correctly, such as control characters and special characters.

If 63 ( 0x3F , '?' ) Is set, "hour, minute, second" will be the delimiter. If set to 0 , the OS setting value will be set.
The initial value is the OS setting value.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type ">property inheritance</a> for time cells .

use case
```
Col = 3;
Row = 2;
CellType = $CellTypeTime;
TypeTimeSeconds = $TRUE;
TypeTimeSeparator = 0x3F; /* '?' */
Value = str(sysdate(), "HHMISS");
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypeTime;
TypeTimeSeparator = 0x2D; /* '-' */
Value = str(sysdate(), "HHMISS");
BlockMode = $FALSE;
```

Related item

<a href="/package/extension5/sspread/properties/celltype">CellType</a> , <a href="/package/extension5/sspread/properties/typetimeseconds">TypeTimeSeconds</a> property