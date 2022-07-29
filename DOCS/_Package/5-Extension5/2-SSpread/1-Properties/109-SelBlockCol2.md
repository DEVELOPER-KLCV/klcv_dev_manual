---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.SelBlockCol2 Property
nav_order: 109
permalink: /package/extension5/sspread/properties/selblockcol2
---
# {{ page.title }}

Refers to the rightmost column number of the selected cell block.

This property is read-only. The initial value is 0.

You can get the position of the selected cell block in combination with the <a href="/package/extension5/sspread/properties/selblockcol">SelBlockCol</a>, <a href="/package/extension5/sspread/properties/selblockrow">SelBlockRow</a>, and <a href="/package/extension5/sspread/properties/selblockrow2">SelBlockRow2</a> properties.
If all columns are selected, the SelBlockCol, SelBlockCol2 property will be -1.

To see if a cell block is selected, look at the <a href="/package/extension5/sspread/properties/isblockselected">IsBlockSelected</a> property.
To select a cell block, use the SetSelection method.

Related Items<br>
<a href="/package/extension5/sspread/properties/isblockselected">IsBlockSelected</a>, <a href="/package/extension5/sspread/properties/selblockcol">SelBlockCol</a>, <a href="/package/extension5/sspread/properties/selblockrow">SelBlockRow</a>, <a href="/package/extension5/sspread/properties/selblockrow2">SelBlockRow2</a> properties<br>
<a href="/package/extension5/sspread/methods/setselection">SetSelection</a> method  