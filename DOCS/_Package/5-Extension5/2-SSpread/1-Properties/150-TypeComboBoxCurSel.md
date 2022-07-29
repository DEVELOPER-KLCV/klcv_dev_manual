---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeComboBoxCurSel Property
nav_order: 150
permalink: /package/extension5/sspread/properties/typecomboboxcursel
---
# {{ page.title }}

Set the index number of the item to be selected in a combo box type cell.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeComboBox .
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties etc. to specify the cell of interest.

Specify an index number starting from 0 . The initial value is -1 (unselected).

You can get the number of items in the list with the <a href="/package/extension5/sspread/properties/typecomboboxcount">TypeComboBoxCount</a> property.

<a href="/package/extension5/sspread/properties/celltype#notes-on-property-inheritance-of-combo-box-type-cells">Notes on property inheritance of combo box type cells</a>

Use case
```
Col = 3;
Row = 2;
CellType = $CellTypeComboBox;
TypeComboBoxList = "AAA\tBBB\tCCC\tDDD\tEEE";
TypeComboBoxCurSel = 2;
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypeComboBox;
TypeComboBoxCurSel = 3;
BlockMode = $FALSE;
```

Related item<br>
 <a href="/package/extension5/sspread/properties/celltype">CellType</a> ,  <a href="/package/extension5/sspread/properties/typecomboboxcount">TypeComboBoxCount</a> ,  <a href="/package/extension5/sspread/properties/typecomboboxlist">TypeComboBoxList</a> property
 