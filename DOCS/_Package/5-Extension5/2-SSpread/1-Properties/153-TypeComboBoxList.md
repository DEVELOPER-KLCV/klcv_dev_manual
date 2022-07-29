---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeComboBoxList Property
nav_order: 153
permalink: /package/extension5/sspread/properties/typecomboboxlist
---
# {{ page.title }}

In the combo box type cell, set the list items at once.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeComboBox (combo box type).
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties etc. to specify what to do.

Separate each item in the list with a tab character ( \t ).
The initial value is an empty string.

Setting this property to a blank string ( "" ) sets the combo box list item to one blank item. ( The <a href="/package/extension5/sspread/properties/typecomboboxcount">TypeComboBoxCount</a> property will be 1 )
Use the <a href="/package/extension5/sspread/methods/typecomboboxclear">TypeComboBoxClear</a> method to completely remove list items .

If you want to add only one combobox list item, use the <a href="/package/extension5/sspread/properties/typecomboboxindex">TypeComboBoxIndex</a> , <a href="/package/extension5/sspread/properties/typecomboboxstring">TypeComboBoxString</a> properties.
You can get the number of items in the list with the <a href="/package/extension5/sspread/properties/typecomboboxcount">TypeComboBoxCount</a> property.
Items are removed using the <a href="/package/extension5/sspread/methods/typecomboboxclear">TypeComboBoxClear</a> and <a href="/package/extension5/sspread/methods/typecomboboxremoveitem">TypeComboBoxRemoveItem</a> methods.

<a href="/package/extension5/sspread/properties/celltype#notes-on-property-inheritance-of-combo-box-type-cells">Notes on property inheritance of combo box type cells</a>

Use case
```
Col = 3;
Row = 2;
CellType = $ CellTypeComboBox;
TypeComboBoxList = "AAA\tBBB\tCCC";
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $ CellTypeComboBox;
TypeComboBoxList = "XXX\tYYY\tZZZ";
BlockMode = $FALSE;
```

Related item<br>
 <a href="/package/extension5/sspread/properties/celltype">CellType</a> ,  <a href="/package/extension5/sspread/properties/typecomboboxcount">TypeComboBoxCount</a> , <a href="/package/extension5/sspread/properties/typecomboboxindex">TypeComboBoxIndex</a> , <a href="/package/extension5/sspread/properties/typecomboboxstring">TypeComboBoxString</a> properties
 <br><a href="/package/extension5/sspread/methods/typecomboboxclear">TypeComboBoxClear</a> , <a href="/package/extension5/sspread/methods/typecomboboxremoveitem">TypeComboBoxRemoveItem</a> methods