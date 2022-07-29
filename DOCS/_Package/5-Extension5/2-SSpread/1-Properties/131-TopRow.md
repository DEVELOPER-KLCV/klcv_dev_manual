---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TopRow Property
nav_order: 131
permalink: /package/extension5/sspread/properties/toprow
---
# {{ page.title }}

Set the number of the line to be displayed on the top line. The initial value is 1.

If the row display is freezed with the <a href="/package/extension5/sspread/properties/rowsfrozen">RowsFrozen</a> property, it will be the number of the top column that can be scrolled.

Use the <a href="/package/extension5/sspread/properties/leftcol">LeftCol</a>  property for the leftmost row.
The right and bottom cells can be obtained with the <a href="/package/extension5/sspread/methods/getbottomrightcell">GetBottomRightCell</a> method.
The <a href="/package/extension5/sspread/events/topleftchange">TopLeftChange</a> event is fired when the display area is scrolled.

Related Items<br>
<a href="/package/extension5/sspread/properties/rowsfrozen">RowsFrozen</a>, <a href="/package/extension5/sspread/properties/leftcol">LeftCol</a> property<br>
<a href="/package/extension5/sspread/methods/getbottomrightcell">GetBottomRightCell</a>, <a href="/package/extension5/sspread/methods/showcell">ShowCell</a> method<br>
<a href="/package/extension5/sspread/events/topleftchange">TopLeftChange</a> event