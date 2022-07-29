---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypePictCenter Property
nav_order: 197
permalink: /package/extension5/sspread/properties/typepictcenter
---
# {{ page.title }}

In a picture cell, set whether to center the image in the cell.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypePicture.
<br>Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Specify $TRUE to place the image in the center of the cell and $FALSE to place it in the upper left of the cell .
The initial value is $FALSE .

This property can only be set to center the image, but you can set the horizontal and vertical positions by using the <a href="/package/extension5/sspread/properties/typehalign">TypeHAlign</a> and <a href="/package/extension5/sspread/properties/typevalign">TypeVAlign</a> properties, respectively.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for picture cells .

Use case
```
Col = 3;
Row = 2;
CellType = $CellTypePicture;
TypePictPicture = "img/sample1.png";
TypePictStretch = $TRUE;
TypePictMaintainScale = $TRUE;
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypePicture;
TypePictPicture = "img/sample2.png";
TypePictMaintainScale = $FALSE;
BlockMode = $FALSE;
```

Related item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a>, <a href="/package/extension5/sspread/properties/typehalign">TypeHAlign</a> , <a href="/package/extension5/sspread/properties/typevalign">TypeVAlign</a> properties.