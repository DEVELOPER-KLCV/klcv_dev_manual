---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeTextWordWrap Property
nav_order: 212
permalink: /package/extension5/sspread/properties/typetextwordwrap
---
# {{ page.title }}

Set whether to word wrap the text in the label cell.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $ CellTypeTime .
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Specify $TRUE for word wrap, and $FALSE otherwise .
The initial value is $FALSE .(In the cells of column header and row header, the initial value is $TRUE).

If you set word wrap, text that exceeds the width of the cell will automatically break.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for label cells .

<a href="/package/extension5/sspread/properties/celltype#notes-on-property-inheritance-of-label-type-cells">Notes on property inheritance of label type cells</a>

Example of use
```
Col = 3;
Row = 2;
CellType = $CellTypeStaticText;
TypeTextWordWrap = $TRUE;
Text = "this is a book. this is a pen.";
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypeStaticText;
TypeTextWordWrap = $TRUE;
Text = "あいうえお\nかきくけこ";
BlockMode = $FALSE;
```

Related item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a> property