---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeEditMultiLine Property
nav_order: 175
permalink: /package/extension5/sspread/properties/typeeditmultiline
---
# {{ page.title }}

For text cells, set whether to allow multi-line input in the cell.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeEdit (text type).
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, etc. to specify what you want to process.

Specify $TRUE if you want to allow multiple lines, or $FALSE if you only have a single line .
<br>The initial value is $FALSE .

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for character cells.

### About line feed code
When using multiple lines of data with SSpread, use CR + LF ( \ r \ n , 0x0d + 0x0a ) as the line feed code.<br>Other line feed codes are automatically replaced with CR + LF when editing the cell.

Example of use
```
Col = 3;
Row = 2;
CellType = $ CellTypeEdit;
TypeEditMultiLine = $ TRUE;
Text = "sample";
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $ CellTypeEdit;
TypeEditMultiLine = $ TRUE;
Text = " Ah \ r \ n Kakiku ";
BlockMode = $ FALSE;
```

Related item<br>
 <a href="/package/extension5/sspread/properties/celltype">CellType</a>  property
