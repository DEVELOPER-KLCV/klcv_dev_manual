---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeTextPrefix Property
nav_order: 209
permalink: /package/extension5/sspread/properties/typetextprefix
---
# {{ page.title }}

Set whether to use the "&" character as the underline in the label cell (underline the character immediately after the "&" ).

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a>  property set to $CellTypeStaticText (label type).
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Specify $TRUE to use the "&" character as an underline, or $FALSE to display the "&" character as is.
The initial value is $FALSE .

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for label cells .

<a href="/package/extension5/sspread/properties/celltype#notes-on-property-inheritance-of-label-type-cells">Notes on property inheritance of label type cells.</a>

Example of use
```
Col = 3;
Row = 2;
CellType = $ CellTypeStaticText;
TypeTextPrefix = $ TRUE;
Text = "& File";
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $ CellTypeStaticText;
TypeTextPrefix = $ FALSE;
Text = "A & B & C";
BlockMode = $ FALSE;
```

Related item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a>  property