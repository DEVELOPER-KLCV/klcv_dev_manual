---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeCheckCenter Property
nav_order: 143
permalink: /package/extension5/sspread/properties/typecheckcenter
---
# {{ page.title }}

In a check box type cell, set whether to place the check box in the center of the cell.
 
Only valid for cells with $CellTypeCheckBox (checkbox type) set in the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property.
Before setting this property, use the  <a href="/package/extension5/sspread/properties/col">Col</a> and <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Specify $TRUE to center the checkbox and text in the cell, or $FALSE to place it to the left of the cell. The initial value is $FALSE.

This property only sets whether the checkbox is centered.
The vertical position is set with the <a href="/package/extension5/sspread/properties/typevalign">TypeVAlign</a> property.

If this property is set to $TRUE, the <a href="/package/extension5/sspread/properties/typehalign">TypeHAlign</a> property that specifies the horizontal position is ignored.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for checkbox cells.

Example of usage<br>
```
Col = 3;
Row = 2;
CellType = $CellTypeCheckBox;
TypeCheckCenter = $TRUE;
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypeCheckBox;
TypeCheckCenter = $TRUE;
BlockMode = $FALSE;
```

Related Items<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a>, <a href="/package/extension5/sspread/properties/textchecktextalign">TextCheckTextAlign</a>, <a href="/package/extension5/sspread/properties/typehalign">TypeHAlign</a>, <a href="/package/extension5/sspread/properties/typevalign">TypeVAlign</a> properties