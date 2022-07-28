---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.SelLength Property
nav_order: 115
permalink: /package/extension5/sspread/properties/sellength
---
# {{ page.title }}

Set the number of characters to select with the value being entered in the active cell.

Only valid when the spreadsheet is in input mode (<a href="/package/extension5/sspread/properties/editmode">EditMode</a> property is $ TRUE).
If -1 is specified, it will be selected until the end.

Get and set the selection in combination with the <a href="/package/extension5/sspread/properties/selstart">SelStart</a> property. In addition, it can be combined with the <a href="/package/extension5/sspread/properties/seltext">SelText</a> property to partially replace the value in the active cell.

Example of usage <br>
```
Function OnEditModeOn (e) {
     / * Set the initial position of the cursor to the beginning * /
     SelStart = 0;
     SelLength = 0;
}
```

Related Items<br>
<a href="/package/extension5/sspread/properties/editmode">EditMode</a>, <a href="/package/extension5/sspread/properties/selstart">SelStart</a>, <a href="/package/extension5/sspread/properties/seltext">SelText</a> properties  