---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.GrayAreaBackColor Property
nav_order: 62
permalink: /package/extension5/sspread/properties/grayareabackcolor
---
# {{ page.title }}

Sets the background color of the area without cells (gray area) when scrolling beyond the maximum rows and columns of the spreadsheet.

Specify a <a href="/base/color">color constant</a> or <a href="package/extension5/sspread/#this-classs-unique-color-handling-rrggbb-format">#RRGGBB format</a>. The initial value is $STD (light gray).

Example of usage<br>
```
GrayAreaBackColor = $DBLUE;
GrayAreaBackColor = "#6B818E";
```

Related Items<br>
<a href="/package/extension5/sspread/properties/backcolor">BackColor</a>, <a href="/package/extension5/sspread/properties/noborder">NoBorder</a> property