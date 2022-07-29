---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeCheckType Property
nav_order: 147
permalink: /package/extension5/sspread/properties/typechecktype
---
# {{ page.title }}

In the check box type cell, set the check box type.

Only valid for cells with $CellTypeCheckBox (checkbox type) set in the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property.
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> and <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.
The initial value is a blank character string.

Specify the following values. The initial value is $TypeCheckTypeNormal.

| Constant                 | Value | Description                         |
|--------------------------|:-----:|-------------------------------------|
| $TypeCheckTypeNormal     |   0   | Standard (checked, unchecked)       |
| $TypeCheckTypeThreeState |   1   | 3 states (checked, unchecked, gray) |

The state of the check box can be obtained with the <a href="/package/extension5/sspread/properties/text">Text</a> property and <a href="/package/extension5/sspread/properties/value">Value</a> property.

(Unchecked = "0", checked = "1", gray state = "2")

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for checkbox cells.

Example of usage<br>
```
Col = 3;
Row = 2;
CellType = $CellTypeCheckBox;
TypeCheckType = $TypeCheckTypeThreeState;
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypeCheckBox;
TypeCheckType = $TypeCheckTypeNormal;
BlockMode = $FALSE;
```

Related Items<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a>, <a href="/package/extension5/sspread/properties/text">Text</a>, <a href="/package/extension5/sspread/properties/value">Value</a> properties