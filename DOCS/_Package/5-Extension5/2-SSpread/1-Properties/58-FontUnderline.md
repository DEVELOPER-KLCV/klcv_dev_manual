---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.FontUnderline Property
nav_order: 58
permalink: /package/extension5/sspread/properties/fontunderline
---
# {{ page.title }}
Sets the font style (Underline) of the displayed text.

Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a>, <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

If underlined, specify $TRUE, otherwise specify $FALSE. The initial value is $FALSE.

As this property changes, so does the value of the <a href="/package/extension5/sspread/properties/fontface">FontFace</a> property.

<a href="/package/extension5/sspread/#limits-on-fonts-applied-to-cell-blocks-">Limits on fonts applied to cell blocks</a>


Example of usage<br>
```
Col = 2;
Row = 3;
FontUnderline = $TRUE;
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
FontUnderline = $TRUE;
BlockMode = $FALSE;
```

Related Items<br>
<a href="/package/extension5/sspread/properties/fontbold">FontBold</a>, <a href="/package/extension5/sspread/properties/fontface">FontFace</a>, <a href="/package/extension5/sspread/properties/fontkitalic">FontItalic</a>, <a href="/package/extension5/sspread/properties/fontkind">FontKind</a>, <a href="/package/extension5/sspread/properties/fontname">FontName</a>, <a href="/package/extension5/sspread/properties/fontsize">FontSize</a>, <a href="/package/extension5/sspread/properties/fontstrikethru">FontStrikethru</a> property