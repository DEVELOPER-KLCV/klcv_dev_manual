---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.FontItalic Property
nav_order: 53
permalink: /package/extension5/sspread/properties/fontitalic
---
# {{ page.title }}

Sets the font style (italic) of the displayed text.

Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a>, <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Specify $TRUE for italic, and $FALSE otherwise. The initial value is $FALSE.

As this property changes, so does the value of the <a href="/package/extension5/sspread/properties/fontface">FontFace</a> property.

<a href="/package/extension5/sspread/#limits-on-fonts-applied-to-cell-blocks-">Limits on fonts applied to cell blocks</a>

Example of usage<br>
```
Col = 2;
Row = 3;
FontItalic = $TRUE;
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
FontItalic = $TRUE;
BlockMode = $FALSE;
```

Related Items<br>
<a href="/package/extension5/sspread/properties/fontbold">FontBold</a>, <a href="/package/extension5/sspread/properties/fontface">FontFace</a>, <a href="/package/extension5/sspread/properties/fontkind">FontKind</a>, <a href="/package/extension5/sspread/properties/fontname">FontName</a>, <a href="/package/extension5/sspread/properties/fontsize">FontSize</a>, <a href="/package/extension5/sspread/properties/fontstrikethru">FontStrikethru</a>, <a href="/package/extension5/sspread/properties/fontunderline">FontUnderline</a> property