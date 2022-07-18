---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.AllowMultiBlocks Property
nav_order: 9
permalink: /package/extension5/sspread/properties/allowmultiblocks
---
# {{ page.title }}

Set whether to allow the user to select multiple cells or cell blocks.

Specify $TRUE for multiple selections, and $FALSE for all others.

The initial value is $FALSE.

If multiple selections are allowed, user can select multiple cells by holding down the Ctrl key and selecting with the mouse.

Use the AddSelection method to select multiple cell blocks programmatically.

Each cell block selected multiple times can be obtained with the GetSelection method.

The selected number can be obtained with the SelectionCount property.

Related Item<br>
<a href="/package/extension5/sspread/properties/selectioncount">SelectionCount</a> property<br>
<a href="/package/extension5/sspread/methods/addselection">AddSelection</a>, <a href="/package/extension5/sspread/methods/getselection">GetSelection</a> method