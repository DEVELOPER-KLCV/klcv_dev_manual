---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeComboBoxEditable Property
nav_order: 151
permalink: /package/extension5/sspread/properties/typecomboboxeditable
---
# {{ page.title }}

Set whether the display text can be edited in a combo box type cell.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeComboBox (combo box type).
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties etc. to specify what you want to process.

Specify $TRUE if you want the display text to be editable , and $FALSE if you want the display text to always be selected from the list items .
The initial value is $FALSE.

If $TRUE is specified, the display text can be obtained and set with the <a href="/package/extension5/sspread/properties/text">Text</a> property.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> of combo box type cells .

<a href="/package/extension5/sspread/properties/celltype#notes-on-property-inheritance-of-combo-box-type-cells">Notes on property inheritance of combo box type cells</a>

Use case
```
Col = 3;
Row = 2;
CellType = $ CellTypeComboBox;
TypeComboBoxEditable = $TRUE;
TypeComboBoxList = "AAA \ tBBB \ tCCC";
Text = "XYZ";
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $ CellTypeComboBox;
TypeComboBoxEditable = $TRUE;
BlockMode = $ FALSE;
```

Related item<br>
 <a href="/package/extension5/sspread/properties/celltype">CellType</a> ,  <a href="/package/extension5/sspread/properties/text">Text</a>  property