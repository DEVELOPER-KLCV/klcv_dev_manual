---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeComboBoxCount Property
nav_order: 149
permalink: /package/extension5/sspread/properties/typecomboboxcount
---
# {{ page.title }}

In the combo box type cell, refer to the number of items in the list.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeComboBox (combo box type).
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties etc. to specify what to process.

This property is read-only. The initial value is 0 .


The number of displayed items can be set with the <a href="/package/extension5/sspread/properties/typecombomaxdrop">TypeComboBoxMaxDrop</a> property.

Use case
```
Col = 3;
Row = 2;
CellType = $CellTypeComboBox;
TypeComboBoxList = "AAA\tBBB\tCCC\tDDD\tEEE";
print(TypeComboBoxCount, "\n");
```

Related item<br>
 <a href="/package/extension5/sspread/properties/celltype">CellType</a> , <a href="/package/extension5/sspread/properties/typecomboboxlist">TypeComboBoxList</a> , <a href="/package/extension5/sspread/properties/typecomboboxmaxdrop">TypeComboBoxMaxDrop</a> properties
