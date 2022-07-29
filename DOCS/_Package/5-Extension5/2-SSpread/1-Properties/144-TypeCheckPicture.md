---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeCheckPicture Property
nav_order: 144
permalink: /package/extension5/sspread/properties/typecheckpicture
---
# {{ page.title }}

In the check box type cell, set the image of the check box.

Only valid for cells with $CellTypeCheckBox (checkbox type) set in the  <a href="/package/extension5/sspread/properties/celltype">CellType</a> property.
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> and <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

This property is an <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a>. For the index, specify the state of the check box from the following values.

| Index | Description                      |
|:-----:|----------------------------------|
|   0   | No checkmark/button not pressed  |
|   1   | With checkmark/No button pressed |
|   2   | No checkmark/button pressed      |
|   3   | With checkmark/Button pressed    |
|   4   | Grayed out/button not pressed    |
|   5   | Grayed out/button pressed        |

Gray display (indexes 4 and 5) is valid only when  <a href="/package/extension5/sspread/properties/typechecktype">TypeCheckType</a>  is $TypeCheckTypeThreeState.

Specify the URL string of the image file or the <a href="/base/readerwriter#reader-object">ReaderObject</a>.
Specify null to cancel the image settings.
This property is for configuration only. It always returns null when it gets a value.

If specify a URL, the file will be cached on users local computer for faster loading from the next time onwards.
The latest files can always be obtained from the server by specifying the <a href="/package/httppackage/httpresponse">HttpResponse</a> object.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for checkbox cells.

Example of usage<br>
```
Col = 3;
Row = 2;
CellType = $CellTypeCheckBox;
TypeCheckPicture(0) = "img/c0.png"; /* Will be cached */
TypeCheckPicture(1) = "img/c1.png";
TypeCheckPicture(2) = "img/c2.png";
TypeCheckPicture(3) = "img/c3.png";
 
var session = getHttpSession();
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypeCheckBox;
TypeCheckPicture(0) = session.Get("img/c0.png"); /* Not cached */
TypeCheckPicture(1) = session.Get("img/c1.png");
TypeCheckPicture(2) = session.Get("img/c2.png");
TypeCheckPicture(3) = session.Get("img/c3.png");
BlockMode = $FALSE;
```

Related Items<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a>, <a href="/package/extension5/sspread/properties/typechecktype">TypeCheckType</a> properties<br>
<a href="/package/httppackage/httpresponse">HttpResponse</a> class