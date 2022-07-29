---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeMaxEditLen Property
nav_order: 179
permalink: /package/extension5/sspread/properties/typemaxeditlen
---
# {{ page.title }}

Set the maximum number of characters that can be entered in a cell.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property.
<br>$CellTypeEdit (character type)
<br>$CellTypeComboBox (combo box type)

Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

The initial value is 32000 (character) for the character cell and 150 (character) for the combo box cell .
<br>Negative values ​​are automatically corrected to 0 .
<br>For character cells, specifying 0 prevents you from entering characters ( cancelled ) . For combo box cells, specifying 0 limits the number of characters.
<br>Please note that the operation differs depending on the <a href="/package/extension5/sspread/properties/celltype">Cell Type</a> .

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for character cells and combo box cells .

<a href="/package/extension5/sspread/properties/celltype#notes-on-property-inheritance-of-combo-box-type-cells">Notes on property inheritance of combo box type cells</a>

Example of use
```
Col= 3;
Row = 2;
CellType = $ CellTypeComboBox;
TypeComboBoxEditable = $ TRUE;
TypeMaxEditLen = 20;
 
BlockMode = $ TRUE;
Col= 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $ CellTypeEdit;
TypeMaxEditLen = 50;
BlockMode = $ FALSE;
 
```

Related item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a> property