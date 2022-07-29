---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypePictPicture Property
nav_order: 199
permalink: /package/extension5/sspread/properties/typepictpicture
---
# {{ page.title }}
 
Set the image in the cell at the picture cell,

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypePicture.
<br>Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Specify the URL string of the image file or the <a href="/base/readerwriter#reader-object">ReaderObject</a> .
Specify null to unset the image .
This property is for configuration only. Whenever you get a value, it returns null .

If you specify a URL , the file will be cached on your local computer for faster loading from the next time onwards.
You can always get the latest files from the server by specifying the <a href="/package/httppackage/httpresponse/">HttpResponse</a> object.

To scale the image to fit the cell size, set the <a href="/package/extension5/sspread/properties/typepictstretch">TypePictStretch</a> property to $TRUE .

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for picture cells .

Use case
```
Col = 3;
Row = 2;
CellType = $CellTypePicture;
TypePictPicture = "img / sample1.png"; / * Cached * /
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypePicture;
TypePictPicture = getHttpSession (). Get ("img / sample2.png"); / * Not cached * /
BlockMode = $FALSE;
```

Related item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a>, <a href="/package/extension5/sspread/properties/typepictstretch">TypePictStretch</a> properties.<br><a href="/package/httppackage/httpresponse/">HttpResponse</a> class