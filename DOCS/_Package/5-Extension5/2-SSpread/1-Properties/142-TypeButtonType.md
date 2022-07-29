---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeButtonType Property
nav_order: 142
permalink: /package/extension5/sspread/properties/typebuttontype
---
# {{ page.title }}

In the command button type cell, set the type of command button.

Only valid for cells with $CellTypeButton (command button type) set in the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property.
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> and <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Specify the following values. The initial value is $TypeButtonTypeNormal.

| Constant                | Value | Description                        |
|-------------------------|:-----:|------------------------------------|
| $TypeButtonTypeNormal   |   0   | Standard                           |
| $TypeButtonTypeTwoState |   1   | Maintained Contact (toggle button) |

$TypeButtonTypeTwoState (maintained contact) is a button that holds the pressed state and returns to the original when pressed again. The state of the button can be obtained with the <a href="/package/extension5/sspread/properties/text">Text</a> property and <a href="/package/extension5/sspread/properties/value">Value</a> property. (Not pressed = "0", pressed = "1")

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for command button cells.

Example of usage<br>
```
Col = 3;
Row = 2;
CellType = $CellTypeButton;
TypeButtonType = $TypeButtonTypeTwoState;
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypeButton;
TypeButtonType = $TypeButtonTypeNormal;
BlockMode = $FALSE;
```

Related Items<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a>, <a href="/package/extension5/sspread/properties/text">Text</a>, <a href="/package/extension5/sspread/properties/value">Value</a> properties