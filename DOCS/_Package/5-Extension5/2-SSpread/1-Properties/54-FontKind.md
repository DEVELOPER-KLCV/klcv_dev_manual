---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.FontKind Property
nav_order: 54
permalink: /package/extension5/sspread/properties/fontkind
---
# {{ page.title }}

Sets the type of font used for display text.

Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a>, <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Specify the following values. The initial value is $STD.

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-cqgq{background-color:#c0c0c0;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
.tg .tg-0ss8{background-color:#c0c0c0;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-j5n6{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;vertical-align:top}
.tg .tg-lcf4{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0ss8">Constant</th>
    <th class="tg-cqgq">Value</th>
    <th class="tg-0ss8">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-j5n6">$STD</td>
    <td class="tg-lcf4">0</td>
    <td class="tg-j5n6">Gothic</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$FONT1</td>
    <td class="tg-lcf4">1</td>
    <td class="tg-j5n6">Ming Dynasty</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$FONT2</td>
    <td class="tg-lcf4">2</td>
    <td class="tg-j5n6" rowspan="6">Font set by <a href="/package/standard/root/methods/setfontfamily">Root.SetFontFamily</a> method</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$FONT3</td>
    <td class="tg-lcf4">3</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$FONT4</td>
    <td class="tg-lcf4">4</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$FONT5</td>
    <td class="tg-lcf4">5</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$FONT6</td>
    <td class="tg-lcf4">6</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$FONT7</td>
    <td class="tg-lcf4">7</td>
  </tr>
</tbody>
</table>

In addition to the above, the font name can also be specified as a character string.

As this property changes, so does the value of the <a href="/package/extension5/sspread/properties/fontsize">FontSize</a> property.

<a href="/package/extension5/sspread/#limits-on-fonts-applied-to-cell-blocks-">Limits on fonts applied to cell blocks</a>

**Differences from the FontKind property of other classes**<br>
In addition to $ STD and $ FONT1 to $ FONT7, you can directly specify any font name installed on your computer as a character string.

If you specify a font name of your choice, the font must be installed on each computer you use.

When referencing this property, fonts that cannot be represented by $ STD and $ FONT1 to $ FONT7 return the font name as a character string.

Example of usage<br>
```
Col = 2;
Row = 3;
FontKind = $FONT1;
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
FontKind = $FONT1;
BlockMode = $FALSE;
```

Related Items<br>
<a href="/package/extension5/sspread/properties/fontbold">FontBold</a>, <a href="/package/extension5/sspread/properties/fontface">FontFace</a>, <a href="/package/extension5/sspread/properties/fontkitalic">FontItalic</a>, <a href="/package/extension5/sspread/properties/fontname">FontName</a>, <a href="/package/extension5/sspread/properties/fontsize">FontSize</a>, <a href="/package/extension5/sspread/properties/fontstrikethru">FontStrikethru</a>, <a href="/package/extension5/sspread/properties/fontunderline">FontUnderline</a> property