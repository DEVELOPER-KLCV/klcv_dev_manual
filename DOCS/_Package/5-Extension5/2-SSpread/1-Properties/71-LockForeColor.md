---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.LockForeColor Property
nav_order: 71
permalink: /package/extension5/sspread/properties/lockforecolor
---
# {{ page.title }}

Sets the text color of locked cells.

Specify a <a href="/base/color">color constant</a> or <a href="package/extension5/sspread/#this-classs-unique-color-handling-rrggbb-format">#RRGGBB format</a>. If $STD is specified, the color specified by the <a href="/package/extension5/sspread/properties/forecolor">ForeColor</a> property will be used as it is. The initial value is $STD.

The background color of locked cells is set with the <a href="/package/extension5/sspread/properties/lockbackcolor">LockBackColor</a> property.

The cell lock is set with the <a href="/package/extension5/sspread/properties/lock">Lock</a> and <a href="/package/extension5/sspread/properties/protect">Protect</a> properties.

Example of usage<br>
```
Col = 2;
Row = 3;
Lock = $TRUE;
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
Lock = $TRUE;
BlockMode = $FALSE;
 
Protect = $TRUE;
LockForeColor = $BLUE;
LockBackColor = "#FFE69B";
```

Related Items<br>
<a href="/package/extension5/sspread/properties/forecolor">ForeColor</a>, <a href="/package/extension5/sspread/properties/lock">Lock</a>, <a href="/package/extension5/sspread/properties/lockbackcolor">LockBackColor</a>, <a href="/package/extension5/sspread/properties/protect">Protect</a> property<br>