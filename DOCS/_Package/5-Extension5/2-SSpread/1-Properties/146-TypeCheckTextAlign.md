---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeCheckTextAlign Property
nav_order: 146
permalink: /package/extension5/sspread/properties/typechecktextalign
---
# {{ page.title }}

In a checkbox cell, set whether the text is placed on the right or left side of the checkbox.

Only valid for cells with $CellTypeCheckBox (checkbox type) set in the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property.
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> and <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.
The initial value is a blank character string.

Specify the following values. The initial value is $TypeCheckTextAlignRight.

| Constant                 | Value | Description                         |
|--------------------------|:-----:|-------------------------------------|
| $TypeCheckTextAlignLeft  |   0   | Placed to the left of the checkbox  |
| $TypeCheckTextAlignRight |   1   | Placed to the right of the checkbox |

The position of the text is specified by the <a href="/package/extension5/sspread/properties/typechecktext">TypeCheckText</a> property.

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