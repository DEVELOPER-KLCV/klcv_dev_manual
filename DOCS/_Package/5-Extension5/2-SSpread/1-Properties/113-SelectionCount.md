---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.SelectionCount Property
nav_order: 113
permalink: /package/extension5/sspread/properties/selectioncount
---
# {{ page.title }}

Gets the number of selected cell blocks or the number of rows when multiple rows are selected.

This property is read-only. The initial value is 0.

If the <a href="/package/extension5/sspread/properties/allowmultiblocks">AllowMultiBlocks</a> property is $TRUE, get the number of cell blocks selected.
Each cell block selected multiple times can be obtained with the <a href="/package/extension5/sspread/methods/getselection">GetSelection</a> method.

When the <a href="/package/extension5/sspread/properties/allowmultiblocks">AllowMultiBlocks</a>, <a href="/package/extension5/sspread/properties/operationmode">OperationMode</a> properties<br>
 property is $OperationModeMulti (multiple selection mode) or $OperationModeExtended (extended multiple selection mode), the number of lines when multiple lines are selected is acquired.
The selected line number can be obtained with the <a href="/package/extension5/sspread/methods/getmultiselitem">GetMultiSelItem</a> method.

Related Items<br>
<a href="/package/extension5/sspread/properties/allowmultiblocks">AllowMultiBlocks</a>, <a href="/package/extension5/sspread/properties/operationmode">OperationMode</a> properties<br>
<a href="/package/extension5/sspread/methods/getmultiselitem">GetMultiSelItem</a>, <a href="/package/extension5/sspread/methods/getselection">GetSelection</a>  method  