---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeCheckText Property
nav_order: 145
permalink: /package/extension5/sspread/properties/typechecktext
---
# {{ page.title }}

In a checkbox cell, set the text to display with the checkbox.

Only valid for cells with $CellTypeCheckBox (checkbox type) set in the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property.
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> and <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.
The initial value is a blank character string.

The position of the text is specified by the <a href="/package/extension5/sspread/properties/typechecktextalign">TypeCheckTextAlign</a> property.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for checkbox cells.

Example of usage<br> 
```
Col = 3;
Row = 2;
CellType = $CellTypeCheckBox;
TypeCheckText = "Check1";
TypeCheckTextAlign = $TypeCheckTextAlignRight;
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypeCheckBox;
TypeCheckText = "Check2";
TypeCheckTextAlign = $TypeCheckTextAlignLeft;
BlockMode = $FALSE;
```

Related Items<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a>, <a href="/package/extension5/sspread/properties/typechecktextalign">TypeCheckTextAlign</a> properties<br>