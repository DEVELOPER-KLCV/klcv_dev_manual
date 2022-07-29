---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeTextShadow Property
nav_order: 210
permalink: /package/extension5/sspread/properties/typetextshadow
---
# {{ page.title }}

In the label type cell, set whether to display the cell so that it looks convex.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a>  property set to $CellTypeStaticText (label type).
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Specify $TRUE if you want it to look convex, otherwise specify $FALSE .
The initial value is $FALSE.(In the cells of column header and row header, the initial value is $TRUE )

Set the <a href="/package/extension5/sspread/properties/typetextshadowin">TypeTextShadowIn</a> property if you want the cells to appear concave .
If you set both the TypeTextShadow and TypeTextShadowIn properties to $TRUE , the TypeTextShadow property takes precedence.

You can use the <a href="/package/extension5/sspread/properties/shadowcolor">ShadowColor</a> , <a href="/package/extension5/sspread/properties/shadowdark">ShadowDark</a> , <a href="/package/extension5/sspread/properties/shadowlight">ShadowLight</a> , <a href="/package/extension5/sspread/properties/shadowtext">ShadowText</a> properties to set the uneven design.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for label cells .

<a href="/package/extension5/sspread/properties/celltype#notes-on-property-inheritance-of-label-type-cells">Notes on property inheritance of label type cells.</a>

Example of use
```
Col = 3;
Row = 2;
CellType = $ CellTypeStaticText;
TypeTextShadow = $ TRUE;
TypeTextShadowIn = $ FALSE;
Text = "sample";
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $ CellTypeStaticText;
TypeTextShadow = $ FALSE;
TypeTextShadowIn = $ TRUE;
Text = "sample";
BlockMode = $ FALSE;
```

Related item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a>  , <a href="/package/extension5/sspread/properties/shadowcolor">ShadowColor</a> , <a href="/package/extension5/sspread/properties/shadowdark">ShadowDark</a> , <a href="/package/extension5/sspread/properties/shadowlight">ShadowLight</a> , <a href="/package/extension5/sspread/properties/shadowtext">ShadowText</a> , <a href="/package/extension5/sspread/properties/typetextshadowin">TypeTextShadowIn</a> properties