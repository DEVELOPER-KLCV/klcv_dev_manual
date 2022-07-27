---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.RowHidden Property
nav_order: 94
permalink: /package/extension5/sspread/properties/rowhidden
---
# {{ page.title }}

Sets whether to hide the row.

Before setting this property, use the <a href="/package/extension5/sspread/properties/row">Row</a> property to specify the desired row.

Specify $TRUE to hide the row and $FALSE to show the row. The initial value is $FALSE.

Set the <a href="/package/extension5/sspread/properties/colhidden">ColHidden</a> property to hide the row.

Example of usage<br>
```
Row = 3;
RowHidden = $TRUE;
```

Related Item<br>
<a href="/package/extension5/sspread/properties/colhidden">ColHidden</a> property