---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.CellNote Property
nav_order: 24
permalink: /package/extension5/sspread/properties/cellnote
---
# {{ page.title }}

Comment on entire spreadsheets and cells in rows, columns, cells, and cell blocks.

A red comment mark is displayed in the upper right corner of the cell where the comment is set, and the comment set is popped up by hovering the mouse over it.

Set a blank string to remove the comment.

Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a>, <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

The initial value is a blank string. <br><small><span style="color:red">Added since Ver.5.0.2</span></small>

Example of usage<br>
```
Col = 2;
Row = 3;
CellNote = "Comment";
 
Col = 2;
Row = 3;
print(CellNote, "\n");
```
