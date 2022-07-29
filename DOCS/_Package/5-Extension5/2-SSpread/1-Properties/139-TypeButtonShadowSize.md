---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeButtonShadowSize Property
nav_order: 139
permalink: /package/extension5/sspread/properties/typebuttonshadowsize
---
# {{ page.title }}

In the command button type cell, set the depth of the bump of the command button.

Only valid for standard styles, such as when the <a href="/package/extension5/sspread/properties/usevisualstyles">UseVisualStyles</a> property is $UseVisualStylesNo (do not use visual styles).

Only valid for cells with $CellTypeButton (command button type) set in the CellType property.

Before setting this property, use <a href="/package/extension5/sspread/properties/col">Col</a> and <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

The initial value is 1.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type"> for command button cells.

***Command button color setting properties***

<a href="/img/Package/Ext5-SSpread-TypeButtonShadowSize.PNG" target="_blank">
<img src="/img/Package/Ext5-SSpread-TypeButtonShadowSize.PNG" alt="login image">

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
<a href="/package/extension5/sspread/properties/apperancestyle">AppearanceStyle</a>,<a href="/package/extension5/sspread/properties/celltype">CellType</a>, <a href="/package/extension5/sspread/properties/typebuttoncolor">TypeButtonColor</a>, <a href="/package/extension5/sspread/properties/typebuttondarkcolor">TypeButtonDarkColor</a>, <a href="/package/extension5/sspread/properties/typebuttonlightcolor">TypeButtonLightColor</a>, <a href="/package/extension5/sspread/properties/typebuttontextcolor">TypeButtonTextColor</a>, <a href="/package/extension5/sspread/properties/usevisualstyles">UseVisualStyles</a> properties