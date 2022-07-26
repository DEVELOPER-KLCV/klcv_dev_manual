---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.Protect Property
nav_order: 84
permalink: /package/extension5/sspread/properties/protect
---
# {{ page.title }}

Sets whether to enable write protection for locked cells.


Specify the following values. The initial value is $TRUE.

| Constant | Description                                                            |
|----------|------------------------------------------------------------------------|
| $TRUE    | Enable write protection to protect cells with a <a href="/package/extension5/sspread/properties/lock">Lock</a> property of $TRUE |
| $FALSE   | Disable write protection                                               |

Example of usage<br>
```
Protect = $ TRUE;
Col = 2;
Row = 3;
Lock = $ TRUE;
```

Related Item<br>
<a href="/package/extension5/sspread/properties/lock">Lock</a> property