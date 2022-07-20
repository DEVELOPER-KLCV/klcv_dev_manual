---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.ColHidden Property
nav_order: 35
permalink: /package/extension5/sspread/properties/colhidden
---
# {{ page.title }}

Set whether to hide the column.

Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> property to specify the target column.

Specify $TRUE to hide the column and $FALSE to show the column. The initial value is $FALSE.

Set the <a href="/package/extension5/sspread/properties/rowhidden">RowHidden</a> property to hide the row.

Example of usage<br>
```
Col = 3;
ColHidden = $TRUE;
```

Related Item<br>
<a href="/package/extension5/sspread/properties/rowhidden">RowHidden</a> property