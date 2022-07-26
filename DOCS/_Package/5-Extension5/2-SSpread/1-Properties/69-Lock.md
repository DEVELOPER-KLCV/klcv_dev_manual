---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.Lock Property
nav_order: 69
permalink: /package/extension5/sspread/properties/lock
---
# {{ page.title }}

Sets whether to lock the entire spreadsheet, rows, columns, cells, or cell blocks (Prevents cell values from being entered or changed).

Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a>, <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Only valid if the <a href="/package/extension5/sspread/properties/protect">Protect</a> property is $TRUE.

Specify $TRUE to lock, or $FALSE otherwise. The initial value is $FALSE.

The color of the locked cell can be changed with the <a href="/package/extension5/sspread/properties/lockforecolor">LockForeColor</a> and <a href="/package/extension5/sspread/properties/lockbackcolor">LockBackColor</a> properties.

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
<a href="/package/extension5/sspread/properties/lockforecolor">LockForeColor</a>, <a href="/package/extension5/sspread/properties/lockbackcolor">LockBackColor</a>, <a href="/package/extension5/sspread/properties/protect">Protect</a> property<br>