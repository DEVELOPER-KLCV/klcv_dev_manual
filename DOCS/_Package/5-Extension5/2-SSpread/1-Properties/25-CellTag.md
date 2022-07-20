---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.CellTag Property
nav_order: 25
permalink: /package/extension5/sspread/properties/celltag
---
# {{ page.title }}

Sets user-defined tags for the specified cells, columns, and rows. This property has no effect on the behavior of the spreadsheet. It can be used for any purpose.

Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a>, <a href="/package/extension5/sspread/properties/row">Row</a> properties to specify the cells, rows, and columns of interest. (The cell block cannot be specified.) The initial value is a blank character string.

Similar features include the <a href="/package/extension5/sspread/methods/setcolitemdata">SetColItemData</a> and <a href="/package/extension5/sspread/methods/setrowitemdata">SetRowItemData</a> methods. These can be set to any numerical data by specifying the row number and column number.

Example of usage<br>
```
Col = 2;
Row = 3;
CellTag = "sample";
 
Col = 2;
Row = 3;
print(CellTag, "\n");
```
Related Items<br>
<a href="/package/extension5/sspread/methods/getcolitemdata">GetColItemData</a>, <a href="/package/extension5/sspread/methods/getrowitemdata">GetRowItemData</a>, <a href="/package/extension5/sspread/methods/setcolitemdata">SetColItemData</a>, <a href="/package/extension5/sspread/methods/setrowitemdata">SetRowItemData</a> method
