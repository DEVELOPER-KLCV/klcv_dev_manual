---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeComboBoxMaxDrop Property
nav_order: 154
permalink: /package/extension5/sspread/properties/typecomboboxmaxdrop
---
# {{ page.title }}

In the combo box cell, set the maximum number of rows to display in the list.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeComboBox.
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties etc. to specify what to do.

If the number of items in the list is greater than the value of this property, the list will display a scrollbar.

The initial value is 6 .

You can get the number of items in the list with the <a href="/package/extension5/sspread/properties/typecomboboxcount">TypeComboBoxCount</a> property.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance </a>of combo box type cells .
<a href="/package/extension5/sspread/properties/celltype#notes-on-property-inheritance-of-combo-box-type-cells">Notes on property inheritance of combo box type cells</a>

Use case
```
Col = 3;
Row = 2;
CellType = $ CellTypeComboBox;
TypeComboBoxList = "AAA\tBBB\tCCC\tDDD\tEEE";
TypeComboBoxMaxDrop = 3;
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $ CellTypeComboBox;
TypeComboBoxMaxDrop = 4;
BlockMode = $FALSE;
```

Related item<br>
 <a href="/package/extension5/sspread/properties/celltype">CellType</a> ,  <a href="/package/extension5/sspread/properties/typecomboboxcount">TypeComboBoxCount</a> properties
