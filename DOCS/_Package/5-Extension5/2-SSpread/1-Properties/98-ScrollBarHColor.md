---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.ScrollBarHColor Property
nav_order: 98
permalink: /package/extension5/sspread/properties/scrollbarhcolor
---
# {{ page.title }}

Sets the background color of the horizontal scroll bar.

Only valid for standard style scrollbars, such as the <a href="/package/extension5/sspread/properties/appearancestyle">AppearanceStyle</a> property for $AppearanceStyleClassic (standard style) and the <a href="/package/extension5/sspread/properties/scrollbarstyle">ScrollBarStyle</a> property for $ScrollBarStyleClassic (standard style).

Specify a <a href="/base/color">color constant</a> or 
<a href="package/extension5/sspread/#this-classs-unique-color-handling-rrggbb-format">#RRGGBB format</a>.
The initial value is $STD (system standard color).

The vertical scroll bar is set with the <a href="/package/extension5/sspread/properties/scrollbarvcolor">ScrollBarVColor</a> property.

Example of usage <br>
```
ScrollBarStyle = $ScrollBarStyleClassic;
ScrollBarHColor = $DMAGENTA;
ScrollBarVColor = "#B271A7";
```

Related Items<br>
<a href="/package/extension5/sspread/properties/appearancestyle">AppearanceStyle</a>, <a href="/package/extension5/sspread/properties/scrollbars">ScrollBars</a>, <a href="/package/extension5/sspread/properties/scrollbarstyle">ScrollBarStyle</a>, <a href="/package/extension5/sspread/properties/scrollbarvcolor">ScrollBarVColor</a> property 