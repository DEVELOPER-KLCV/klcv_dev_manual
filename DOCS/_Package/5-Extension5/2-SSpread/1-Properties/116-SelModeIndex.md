---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.SelModeIndex Property
nav_order: 116
permalink: /package/extension5/sspread/properties/selmodeindex
---
# {{ page.title }}

Sets the line number to select when the <a href="/package/extension5/sspread/properties/operationmode">OperationMode</a>  property is $OperationModeSingle.

Example of usage<br>
```
OperationMode = $OperationModeSingle;
Function OnRClicked(e) {
    SelModeIndex = e.Row;
}
```

Related Items<br>
<a href="/package/extension5/sspread/properties/operationmode">OperationMode</a> property