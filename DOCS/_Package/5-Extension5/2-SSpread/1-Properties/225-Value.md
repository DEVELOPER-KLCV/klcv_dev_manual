---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.Value Property
nav_order: 225
permalink: /package/extension5/sspread/properties/value
---
# {{ page.title }}

Set values ​​such as strings, numbers, and dates in cells.

Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

The initial value is a blank character string.

The rules for getting and setting this property differ depending on the cell data type ( <a href= "/package/extension5/sspread/properties/celltype">CellType</a> property).

For details , refer to <a href="/package/extension5/sspread/#get-and-set-the-value-for-each-cell-data-type-">Obtaining and setting values ​​for each cell data type</a> .

You can get the unformatted string with the Value property and the formatted string with the <a href="/package/extension5/sspread/properties/text">Text</a> property.

Example of use
```
Col = 2;
Row = 3;
Value = "sample1";
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
Value = "sample2";
BlockMode = $ FALSE;
 ```
Related item
<a href="/package/extension5/sspread/properties/celltype">CellType</a> , <a href="/package/extension5/sspread/properties/clipvalue">ClipValue</a> , <a href="/package/extension5/sspread/properties/text">Text</a> properties