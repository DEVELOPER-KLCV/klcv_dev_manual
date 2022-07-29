---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeEditPassword Property
nav_order: 176
permalink: /package/extension5/sspread/properties/typeeditpassword
---
# {{ page.title }}

In the character cell, set whether to use the password display format ( * is displayed instead of the entered characters).

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeEdit (character type).
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, etc. to specify what you want to process.

Disabled if the <a href="/package/extension5/sspread/properties/typeeditmultiline">TypeEditMultiLine</a> property is set to $TRUE .

Specify $TRUE to use the display format for passwords, otherwise specify $FALSE .
<br>The initial value is $FALSE .

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for character cells.

Example of use
```
Col = 3;
Row = 2;
CellType = $CellTypeEdit;
TypeEditPassword = $ TRUE;
Text = "sample";
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypeEdit;
TypeEditPassword = $ TRUE;
Text = "abc";
BlockMode = $ FALSE;
```

Related item<br>
 <a href="/package/extension5/sspread/properties/celltype">CellType</a> , <a href="/package/extension5/sspread/properties/typeeditmultiline">TypeEditMultiLine</a> property
