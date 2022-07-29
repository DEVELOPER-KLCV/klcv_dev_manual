---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypePictStretch Property
nav_order: 200
permalink: /package/extension5/sspread/properties/typepictstretch
---
# {{ page.title }}
In the picture cell, set whether to enlarge or reduce the image according to the size of the cell.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypePicture.
<br>Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Specify $TRUE to enlarge or reduce the image, and $FALSE to display it in its original size.
The initial value is $FALSE.

The image to be displayed is set by the <a href="/package/extension5/sspread/properties/typepictpicture">TypePictPicture</a> property.
Set the <a href="/package/extension5/sspread/properties/typepictmaintainscale">TypePictMaintainScale</a> property to $ TRUE to maintain the aspect ratio of the image when zooming in and out.

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
TypePictStretch = $FALSE;
BlockMode = $FALSE;
```

Related item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a>, <a href="/package/extension5/sspread/properties/typepictmaintainscale">TypePictMaintainScale</a>, <a href="/package/extension5/sspread/properties/typepictpicture">TypePictPicture</a> property.