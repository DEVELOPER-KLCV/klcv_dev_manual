---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.SelModeSelected Property
nav_order: 117
permalink: /package/extension5/sspread/properties/selmodeselected
---
# {{ page.title }}

Set whether to select the row indicated by the Row property when the OperationMode property is $OperationModeMulti (multi-select mode) or $ OperationModeExtended (extended multiple-select mode).

Specify $TRUE to select it, and $FALSE otherwise.

The number of selected rows can be obtained with the SelectionCount property.
The selected line number can be obtained with the GetMultiSelItem method.

Example of usage<br>
```
OperationMode = $OperationModeMulti;
Row = 2;
SelModeSelected = $TRUE;
Row = 4;
SelModeSelected = $TRUE;
Row = 6;
SelModeSelected = $TRUE;
```

Related Items<br>
<a href="/package/extension5/sspread/properties/operationmode">OperationMode</a>,
<a href="/package/extension5/sspread/properties/selectioncount">SelectionCount</a> properties<br>
<a href="/package/extension5/sspread/properties/getmultiselitem">GetMultiSelItem</a> method