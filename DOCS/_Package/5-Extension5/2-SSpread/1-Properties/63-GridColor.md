---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.GridColor Property
nav_order: 63
permalink: /package/extension5/sspread/properties/gridcolor
---
# {{ page.title }}

Sets the color of the grid lines in the spreadsheet.

Specify a <a href="/base/color">color constant</a> or <a href="package/extension5/sspread/#this-classs-unique-color-handling-rrggbb-format">#RRGGBB format</a>. The initial value is $ STD (light gray).

To show / hide the grid lines, use the <a href="/package/extension5/sspread/properties/gridshowhoriz">GridShowHoriz</a> and <a href="/package/extension5/sspread/properties/gridshowvert">GridShowVert</a> properties.

The grid line type can be set with the <a href="/package/extension5/sspread/properties/gridsolid">GridSolid</a> property.

In the initial state, the grid lines are filled with the background color of the cells specified by the <a href="/package/extension5/sspread/properties/backcolor">BackColor</a> property. The display order of the background color and grid lines can be changed with the <a href="/package/extension5/sspread/properties/backcolorstyle">BackColorStyle</a> property.

Example of usage<br>
```
GridColor = $DCYAN;
GridColor = "#007CA0";
```

Related Items<br>
<a href="/package/extension5/sspread/properties/backcolor">BackColor</a>, <a href="/package/extension5/sspread/properties/backcolorstyle">BackColorStyle</a>, <a href="/package/extension5/sspread/properties/gridshowhoriz">GridShowHoriz</a>, <a href="/package/extension5/sspread/properties/gridshowvert">GridShowVert</a>, <a href="/package/extension5/sspread/properties/gridsolid">GridSolid</a> property