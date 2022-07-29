---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeComboBoxString Property
nav_order: 155
permalink: /package/extension5/sspread/properties/typecomboboxstring
---
# {{ page.title }}

Get and add list items in the combo box type cell.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeComboBox (combo box type).
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties etc.

The index number set in the <a href="/package/extension5/sspread/properties/row">Row</a>TypeComboBoxIndex property will be processed.

The index number set in the <a href="/package/extension5/sspread/properties/typecomboboxindex">TypeComboBoxIndex</a> property will be processed.
When you refer to the value of the property, get the target one from the list item .
When you assign a value to the property, add a new item at the target position of the list item. If the TypeComboBoxIndex property is -1 , add it to the end of the list items.


If you want to edit the list items of the combo box in bulk, use the <a href="/package/extension5/sspread/properties/typecomboboxlist">TypeComboBoxList</a> property.
You can get the number of items in the list with the <a href="/package/extension5/sspread/properties/typecomboboxcount">TypeComboBoxCount</a> property.

Items can be deleted with the <a href="/package/extension5/sspread/methods/typecomboboxclear">TypeComboBoxClear</a> and <a href="/package/extension5/sspread/methods/typecomboboxremoveitem">TypeComboBoxRemoveItem</a> methods.

<a href="/package/extension5/sspread/properties/celltype#notes-on-property-inheritance-of-combo-box-type-cells">Notes on property inheritance of combo box type cells</a>

Use case
```
Col = 3;
Row = 2;
CellType = $ CellTypeComboBox;
TypeComboBoxIndex = 0;
TypeComboBoxString = "AAA";
TypeComboBoxIndex = 1;
TypeComboBoxString = "BBB";
TypeComboBoxIndex = 2;
TypeComboBoxString = "CCC";
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $ CellTypeComboBox;
TypeComboBoxIndex = 0;
TypeComboBoxString = "XXX";
TypeComboBoxIndex = 1;
TypeComboBoxString = "YYY";
TypeComboBoxIndex = 2;
TypeComboBoxString = "ZZZ";
BlockMode = $FALSE;
```

Related item<br>
 <a href="/package/extension5/sspread/properties/celltype">CellType</a> ,  <a href="/package/extension5/sspread/properties/typecomboboxcount">TypeComboBoxCount</a> , <a href="/package/extension5/sspread/properties/typecomboboxindex">TypeComboBoxIndex</a> , <a href="/package/extension5/sspread/properties/typecomboboxlist">TypeComboBoxList</a> properties
 <br><a href="/package/extension5/sspread/methods/typecomboboxclear">TypeComboBoxClear</a> , <a href="/package/extension5/sspread/methods/typecomboboxremoveitem">TypeComboBoxRemoveItem</a> methods