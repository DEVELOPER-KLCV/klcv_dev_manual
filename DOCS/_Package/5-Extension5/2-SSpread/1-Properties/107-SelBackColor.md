---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.SelBackColor Property
nav_order: 107
permalink: /package/extension5/sspread/properties/selbackcolor
---
# {{ page.title }}

Sets the background color of the selected cell block.

Specify a <a href="/base/color">color constant</a> or
<a href="package/extension5/sspread/#this-classs-unique-color-handling-rrggbb-format">#RRGGBB format</a>.

The behavior when $STD is specified depends on the setting of the <a href="/package/extension5/sspread/properties/appearancestyle">AppearanceStyle</a> property. In the case of $AppearanceStyleClassic (standard style), it will be the reverse color of the background color specified by the <a href="/package/extension5/sspread/properties/backcolor">BackColor</a> property. For other styles, it is based on the color of the selection set in the system.

The initial value is $STD.

The text color of the selected cell is set with the <a href="/package/extension5/sspread/properties/selforecolor">SelForeColor</a> property.

Example of usage<br>
```
SelForeColor = $DGREEN;
SelBackColor = "#F2ED71";
```

Related Items<br>
<a href="/package/extension5/sspread/properties/appearancestyle">AppearanceStyle</a>, <a href="/package/extension5/sspread/properties/backcolor">BackColor</a>, <a href="/package/extension5/sspread/properties/selforecolor">SelForeColor</a> properties  