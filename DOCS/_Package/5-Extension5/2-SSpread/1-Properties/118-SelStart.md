---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.SelStart Property
nav_order: 118
permalink: /package/extension5/sspread/properties/selstart
---
# {{ page.title }}

The value entered in the active cell sets the starting position for the selection.

Only valid when the spreadsheet is in input mode (<a href="/package/extension5/sspread/properties/editmode">EditMode</a> property is $TRUE).

Get and set the selection in combination with the <a href="/package/extension5/sspread/properties/sellength">SelLength</a> property. In addition, it can be combined with the  <a href="/package/extension5/sspread/properties/seltext">SelText</a> property to partially replace the value in the active cell.

Example of usage<br>
```
Function OnEditModeOn (e) {
     / * Set the initial position of the cursor to the beginning * /
     SelStart = 0;
     SelLength = 0;
}
```

Related Items<br>
<a href="/package/extension5/sspread/properties/editmode">EditMode</a>, <a href="/package/extension5/sspread/properties/sellength">SelLength</a>, <a href="/package/extension5/sspread/properties/seltext">SelText</a> properties  