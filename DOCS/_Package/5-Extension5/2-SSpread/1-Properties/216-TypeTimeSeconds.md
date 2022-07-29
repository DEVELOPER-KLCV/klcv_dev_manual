---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeTimeSeconds Property
nav_order: 216
permalink: /package/extension5/sspread/properties/typetimeseconds
---
# {{ page.title }}
Set whether to display seconds in the time cell.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeTime .
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Specify $TRUE to display seconds and $FALSE to not display them.

The initial value is $FALSE .

The time format is set with the <a href= "/package/extension5/sspread/properties/typetime24hour">TypeTime24Hour</a> property.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type ">property inheritance</a> for time cells .

Example of use
```
Col = 3;
Row = 2;
CellType = $ CellTypeTime;
TypeTimeSeconds = $ TRUE;
Value = str (sysdate (), "HHMISS");
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $ CellTypeTime;
TypeTimeSeconds = $ FALSE;
Value = str (sysdate (), "HHMISS");
BlockMode = $ FALSE;
```

Related item

<a href="/package/extension5/sspread/properties/celltype">CellType</a> , <a href= "/package/extension5/sspread/properties/typetime24hour">TypeTime24Hour</a> property