---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeButtonPicture Property
nav_order: 137
permalink: /package/extension5/sspread/properties/typebuttonpicture
---
# {{ page.title }}

In the command button cell, set the color of the lower right side of the bump of the command button.

Only valid for standard styles, such as when the <a href="/package/extension5/sspread/properties/usevisualstyles">UseVisualStyles</a> property is $UseVisualStylesNo (do not use visual styles).

Only valid for cells with $CellTypeButton (command button type) set in the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property.
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> and <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Specify a <a href="/base/color">color constant</a> or <a href="package/extension5/sspread/#this-classs-unique-color-handling-rrggbb-format">#RRGGBB format</a>.
The initial value is the OS setting value. Setting $STD will return to the OS settings.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for command button cells.

***Command button color setting properties***

<a href="/img/Package/Ext5-SSpread-TypeButtonLightColor.PNG" target="_blank">
<img src="/img/Package/Ext5-SSpread-TypeButtonLightColor.PNG" alt="login image">

Example of usage<br>
```
Col = 3;
Row = 2;
CellType = $CellTypeButton;
TypeButtonPicture = "img/sample1.png"; /* Will be cached */
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypeButton;
TypeButtonPicture = getHttpSession().Get("img/sample2.png"); /* Not cached */
BlockMode = $FALSE;
```

Related Items<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a>, <a href="/package/extension5/sspread/properties/typebuttonpicturedown">TypeButtonPictureDown</a> properties<br>
<a href="/package/httppackage/httpresponse">HttpResponse</a> class
