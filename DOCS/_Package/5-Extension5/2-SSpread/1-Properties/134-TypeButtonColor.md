---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeButtonColor Property
nav_order: 134
permalink: /package/extension5/sspread/properties/typebuttoncolor
---
# {{ page.title }}

In the command button cell, set the background color of the command button.

Only valid for standard styles, such as when the <a href="/package/extension5/sspread/properties/usevisualstyles">UseVisualStyles</a> property is $UseVisualStylesNo (do not use visual styles).

Only valid for cells with $CellTypeButton (command button type) set in the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property.
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> and <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Specify a <a href="/base/color">color constant</a> or <a href="package/extension5/sspread/#this-classs-unique-color-handling-rrggbb-format">#RRGGBB format</a>.
The initial value is the OS setting value. Setting $STD will return to the OS settings.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for command button cells.

***Command button color setting properties***

<a href="/img/Package/Ext5-SSpread-TypeButtonColor.PNG" target="_blank">
<img src="/img/Package/Ext5-SSpread-TypeButtonColor.PNG" alt="login image">

Example of usage<br>
```
UseVisualStyles = $UseVisualStylesNo;
Col = 2;
Row = 2;
CellType = $CellTypeButton;
TypeButtonText = "Button1";
TypeButtonColor = $DCYAN;
TypeButtonTextColor = $WHITE;
TypeButtonLightColor = "#DAEAD0";
TypeButtonDarkColor = "#005C50";
TypeButtonShadowSize = 4;
 
Col = 2;
Row = 4;
CellType = $CellTypeButton;
 
Col = 2;
Row = 6;
CellType = $CellTypeButton;
 
BlockMode = $TRUE;
Col = 4;
Row = 3;
Col2 = 4;
Row2 = 5;
CellType = $CellTypeButton;
BlockMode = $FALSE;
```

Related Items<br>
<a href="/package/extension5/sspread/properties/apperancestyle">AppearanceStyle</a>,<a href="/package/extension5/sspread/properties/celltype">CellType</a>, <a href="/package/extension5/sspread/properties/typebuttondarkcolor">TypeButtonDarkColor</a>, <a href="/package/extension5/sspread/properties/typebuttonlightcolor">TypeButtonLightColor</a>, <a href="/package/extension5/sspread/properties/typebuttonshadowsize">TypeButtonShadowSize</a>, <a href="/package/extension5/sspread/properties/typebuttontextcolor">TypeButtonTextColor</a>, <a href="/package/extension5/sspread/properties/usevisualstyles">UseVisualStyles</a> properties