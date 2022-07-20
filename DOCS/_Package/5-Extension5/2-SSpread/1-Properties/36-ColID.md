---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.ColID Property
nav_order: 36
permalink: /package/extension5/sspread/properties/colid
---
# {{ page.title }}

Sets a string that can be used to identify the column for a particular column.

Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> property to specify the target column. The initial value is a blank character string.

Setting the ColID property on a column allows you to reference the column using the <a href="/package/extension5/sspread/methods/getcolfromid">GetColFromID</a> method.

Even if the column moves, it can be referenced, so the column can be identified more reliably than the column number.

Example of usage<br>
```
Col = 3;
ColID = "address";
print(GetColFromID("address"), "\n");
```

Related Item<br>
<a href="/package/extension5/sspread/methods/getcolfromid">GetColFromID</a> method