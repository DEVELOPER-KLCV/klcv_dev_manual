---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.BackColor Property
nav_order: 17
permalink: /package/extension5/sspread/properties/backcolor
---
# {{ page.title }}

Sets the background color for the entire spreadsheet, rows, columns, cells, and cell blocks.

Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a>, <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Specify a <a href="/base/color">color constant</a> or <a href="package/extension5/sspread/#this-classs-unique-color-handling-rrggbb-format">#RRGGBB format</a>. The initial value is $WHITE.

Use the <a href="/package/extension5/sspread/methods/setoddevenrowcolor">SetOddEvenRowColor</a> method to set a different color for each row (set different colors for even and odd rows). The color of the locked cell takes precedence over the setting of the <a href="/package/extension5/sspread/methods/lockbackcolor">LockBackColor</a> property.

In the initial state, the background color of the cell is displayed above the grid line. The display order of the background color and grid lines can be changed with the <a href="/package/extension5/sspread/properties/backcolorstyle">BackColor Style</a> property.

Example of usage<br>
```
Col = 2;
Row = 3;
BackColor = $YELLOW;
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
BackColor = "#FFEF90";
BlockMode = $FALSE;
```

Related Items<br>
<a href="/package/extension5/sspread/properties/backcolorstyle">BackColor Style</a>, <a href="/package/extension5/sspread/methods/forecolor">ForeColor</a>, <a href="/package/extension5/sspread/methods/lockbackcolor">LockBackColor</a> property<br> <a href="/package/extension5/sspread/methods/setoddevenrowcolor">SetOddEvenRowColor</a> method