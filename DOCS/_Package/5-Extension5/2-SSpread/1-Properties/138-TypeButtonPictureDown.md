---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeButtonPictureDown Property
nav_order: 138
permalink: /package/extension5/sspread/properties/typebuttonpicturedown
---
# {{ page.title }}

In the command button type cell, set the image when the command button is pressed.

Only valid for cells with $CellTypeButton (command button type) set in the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property.
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> and <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Specify the URL string of the image file or the <a href="/base/readerwriter#reader-object">ReaderObject</a>.
Specify null to cancel the image settings.
This property is for configuration only. It always returns null when it gets a value.

If this property is not specified and the <a href="/package/extension5/sspread/properties/typebuttonpicture">TypeButtonPicture</a> property is specified, the image set by the TypeButtonPicture property will be displayed regardless of the state of the command button.

Specify a URL, the file will be cached on local computer for faster loading from the next time onwards.
The latest files can always be obtained from the server by specifying the <a href="/package/httppackage/httpresponse">HttpResponse</a> object.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for command button cells.

Example of usage<br>
```
Col = 3;
Row = 2;
CellType = $CellTypeButton;
TypeButtonPictureDown = "img/sample1.png"; /* Will be cached */
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypeButton;
TypeButtonPictureDown = getHttpSession().Get("img/sample2.png"); /* Not cached  */
BlockMode = $FALSE;
```

Related Items<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a>, <a href="/package/extension5/sspread/properties/typebuttonpicture">TypeButtonPicture</a> properties<br>
<a href="/package/httppackage/httpresponse">HttpResponse</a> class