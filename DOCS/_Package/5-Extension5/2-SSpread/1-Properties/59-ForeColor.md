---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.ForeColor Property
nav_order: 59
permalink: /package/extension5/sspread/properties/forecolor
---
# {{ page.title }}

Sets the text color for the entire spreadsheet, rows, columns, cells, and cell blocks.

Before setting this property, use the Col, Row properties, and so on to specify what to do.

Specify a <a href="/base/color">color constant</a>  or <a href="package/extension5/sspread/#this-classs-unique-color-handling-rrggbb-format">#RRGGBB format</a>. The initial value is $ BLACK.

Use the <a href="/package/extension5/sspread/methods/setoddevenrowcolor">SetOddEvenRowColor</a>  method to set a different color for each row (set a different color for even and odd rows).

The color of the text in the locked cell takes precedence over the setting of the <a href="/package/extension5/sspread/properties/lockforecolor">LockForeColor</a> property.

Example of usage<br>
```
Col = 2;
Row = 3;
ForeColor = $DRED;
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
ForeColor = "#A93224";
BlockMode = $FALSE;
```

Related Items<br>
<a href="/package/extension5/sspread/properties/backcolor">BackColor</a>, <a href="/package/extension5/sspread/properties/lockforecolor">LockForeColor</a> property<br>
<a href="/package/extension5/sspread/methods/setoddevenrowcolor">SetOddEvenRowColor</a> method