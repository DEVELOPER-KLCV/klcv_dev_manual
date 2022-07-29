---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeButtonText Property
nav_order: 140
permalink: /package/extension5/sspread/properties/typebuttontext
---
# {{ page.title }}

In the command button cell, set the text to be displayed on the command button.


Only valid for cells with $CellTypeButton (command button type) set in the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property.
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> and <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

The initial value is a blank character string.

The text color can be set with the <a href="/package/extension5/sspread/properties/typebuttontextcolor">TypeButtonTextColor</a> property.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for command button cells.

Example of usage<br>
```
Col = 3;
Row = 2;
CellType = $CellTypeButton;
TypeButtonText = "Button1";
TypeButtonTextColor = $DRED;
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypeButton;
TypeButtonText = "Button2";
TypeButtonTextColor = "#893A39";
BlockMode = $FALSE;
```

Related Items<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a>, <a href="/package/extension5/sspread/properties/typebuttontextcolor">TypeButtonTextColor</a> properties