---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeComboBoxIndex Property
nav_order: 152
permalink: /package/extension5/sspread/properties/typecomboboxindex
---
# {{ page.title }}

Set the index number of the list item you want to process before using the <a href="/package/extension5/sspread/properties/typecomboboxstring">TypeComboBoxString</a> property.

Specify an index number starting from 0 . The initial value is 0 .

This property is only a function that holds the value as a variable and does not affect its behavior by itself.
Used only when getting and setting the <a href="/package/extension5/sspread/properties/typecomboboxstring">TypeComboBoxString</a> property.

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
```

Related item<br>
 <a href="/package/extension5/sspread/properties/celltype">CellType</a> ,  <a href="/package/extension5/sspread/properties/typecomboboxstring">TypeComboBoxString</a>  property