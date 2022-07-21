---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.FontName Property
nav_order: 55
permalink: /package/extension5/sspread/properties/fontname
---
# {{ page.title }}

Sets the font name used for the display text.

Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a>, <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do. The initial value is "MS Gothic".

As this property changes, so does the value of the <a href="/package/extension5/sspread/properties/fontkind">FontKind</a> property.

Be sure to specify the font installed on the computer for the font name. If the font is not found, the display result is undefined.


<a href="/package/extension5/sspread/#limits-on-fonts-applied-to-cell-blocks-">Limits on fonts applied to cell blocks</a>


Example of usage<br>
```
Col = 2;
Row = 3;
FontName = "ＭＳ Mincho";
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
FontName = "MS UI Gothic";
BlockMode = $FALSE;
```

Related Items<br>
<a href="/package/extension5/sspread/properties/fontbold">FontBold</a>, <a href="/package/extension5/sspread/properties/fontface">FontFace</a>, <a href="/package/extension5/sspread/properties/fontkitalic">FontItalic</a>, <a href="/package/extension5/sspread/properties/fontkind">FontKind</a>, <a href="/package/extension5/sspread/properties/fontsize">FontSize</a>, <a href="/package/extension5/sspread/properties/fontstrikethru">FontStrikethru</a>, <a href="/package/extension5/sspread/properties/fontunderline">FontUnderline</a> property