---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypePicDefaultText Property
nav_order: 195
permalink: /package/extension5/sspread/properties/typepicdefaulttext
---
# {{ page.title }}

In the mask type cell, set the character string to be displayed as the initial value when the cell is in the edit state.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypePicture.
<br>Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

The initial value is a blank character string.

You can set the character to be displayed as the initial value at the position of the format set by the <a href="/package/extension5/sspread/properties/typepicmask">TypePicMask</a> property, and inform the user of the number of digits to be input and the type of character.
<br>If you delete the entered data, the characters set in this property will be displayed instead of the deleted characters.
<br>If you do not want to display anything, set a blank character string.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for masked cells .

Example of use
```
Col = 3;
Row = 2;
CellType = $ CellTypePic;
TypePicMask = "999-9999";
TypePicDefaultText = "000-0000";
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $ CellTypePic;
TypePicMask = "U99.99.99 ~ U99.99.99";
TypePicDefaultText = "# __ . __. __ ~ # __ .__ .__";
BlockMode = $ FALSE;
```

Related item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a>, <a href="/package/extension5/sspread/properties/typepicmask">TypePicMask</a> properties.