---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.FontFace Property
nav_order: 52
permalink: /package/extension5/sspread/properties/fontface
---
# {{ page.title }}

Sets the font style of the display text.

Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a>, <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Specify a combination of the following values. The initial value is $STD.

| Constant   | Value | Description   |
|------------|:-------:|---------------|
| $STD       | 0     | Standard      |
| $BOLD      | 1     | Bold          |
| $ITALIC    | 2     | Italic        |
| $UNDER     | 4     | Underline     |
| $STRIKEOUT | 16    | Strikethrough |

The values of the <a href="/package/extension5/sspread/properties/fontbold">FontBold</a>, <a href="/package/extension5/sspread/properties/fontitalic">FontItalic</a>,  <a href="/package/extension5/sspread/properties/fontunderline">FontUnderline</a> and <a href="/package/extension5/sspread/properties/fontstrikethru">FontStrikethru</a> properties change as this property changes.

<a href="/package/extension5/sspread/#limits-on-fonts-applied-to-cell-blocks-">Limits on fonts applied to cell blocks</a>

**Differences from the FontFace property of other classes**

$FIXED cannot be used. Specify the monospaced font in the <a href="/package/extension5/sspread/properties/fontname">FontName</a> property to use a monospaced font.
$STRIKEOUT can be specified only for this class.

Example of usage<br>
```
Col = 2;
Row = 3;
FontFace = $ BOLD + $ ITALIC;
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
FontFace = $ STRIKEOUT;
BlockMode = $ FALSE;
```

Related Items<br>
<a href="/package/extension5/sspread/properties/fontbold">FontBold</a>, <a href="/package/extension5/sspread/properties/fontitalic">FontItalic</a>, <a href="/package/extension5/sspread/properties/fontkind">FontKind</a>, <a href="/package/extension5/sspread/properties/fontname">FontName</a>, <a href="/package/extension5/sspread/properties/fontsize">FontSize</a>, <a href="/package/extension5/sspread/properties/fontstrikethru">FontStrikethru</a>, <a href="/package/extension5/sspread/properties/fontunderline">FontUnderline</a> property
