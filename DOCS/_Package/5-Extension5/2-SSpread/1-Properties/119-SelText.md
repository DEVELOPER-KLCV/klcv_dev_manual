---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.SelText Property
nav_order: 119
permalink: /package/extension5/sspread/properties/seltext
---
# {{ page.title }}

Sets the text to select with the value yentered in the active cell.

Only valid when the spreadsheet is in input mode (<a href="/package/extension5/sspread/properties/editmode">EditMode</a> property is $TRUE).

In combination with the <a href="/package/extension5/sspread/properties/selstart">SelStart</a> and <a href="/package/extension5/sspread/properties/sellength">SelLength</a> properties, the value in the active cell can partially replaced. 

Example of usage<br>
```
Function OnEditModeOn (e) {
     / * Set the initial value * /
     SelStart = 0;
     SelLength = -1;
     if (SelText.Length == 0) {
         SelText = sysdate ();
     }
}
```

Related Items<br>
<a href="/package/extension5/sspread/properties/editmode">EditMode</a>, <a href="/package/extension5/sspread/properties/sellength">SelLength</a>, <a href="/package/extension5/sspread/properties/selstart">SelStart</a> properties  